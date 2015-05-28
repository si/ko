#Spodatus Data Schema


##Calendars

	id INT UNIQUE
	name VARCHAR(50)
	description VARCHAR(255)
	default_reminder_mins INT
	status SMALLINT {1:Draft, 2:Live, 3:Archive}
	access SMALLINT {1:Public, 2:Private 3:Invited}
	created DATETIME
	updated DATETIME

##Events

	id INT UNIQUE
	calendar_id INT (FK Calendars.id)
	starts DATETIME
	ends DATETIME
	is_all_day BOOLEAN
	location_id INT (FK Location.id)
	winner_id INT (FK EventTeams.id)
	status SMALLINT {1:Draft, 2:Live, 3:Archive}
	created DATETIME
	updated DATETIME
	
##EventMeta

	id INT UNIQUE
	event_id INT (FK Events.id)
	key VARCHAR(30)
	value VARCHAR(255)
	status SMALLINT {1:Draft, 2:Live, 3:Archive}
	created DATETIME
	updated DATETIME
	
##EventTeams

	id INT UNIQUE
	event_id INT (FK Events.id)
	team_id INT (FK Teams.id)
	order INT
	
##Teams

	id INT UNIQUE
	full_name VARCHAR(30)
	short_name VARCHAR(20)
	logo_id INT (FK Media.id)
	venue_id INT (FK Locations.id)
	status SMALLINT {1:Draft, 2:Live, 3:Archive}
	created DATETIME
	updated DATETIME
	
##TeamSocialAccounts

	id INT UNIQUE
	team_id INT (FK Teams.id)
	social_id INT (FK SocialAccounts.id)
	status SMALLINT {1:Draft, 2:Live, 3:Archive}
	created DATETIME
	updated DATETIME

##Players

	id INT UNIQUE
	team_id INT (FK Teams.id)
	first_name VARCHAR(50)
	last_name VARCHAR(50)
	nick_name VARCHAR(30)
	dob DATE
	number INT
	photo_id INT (FK Media.id)
	status SMALLINT {1:Draft, 2:Live, 3:Archive}
	created DATETIME
	updated DATETIME

##PlayerSocialAccounts

	id INT UNIQUE
	player_id INT (FK Players.id)
	social_id INT (FK SocialAccounts.id)
	status SMALLINT {1:Draft, 2:Live, 3:Archive}
	created DATETIME
	updated DATETIME
	
##Media

	id INT UNIQUE
	path VARCHAR(255)
	size INT
	status SMALLINT {1:Draft, 2:Live, 3:Archive}
	created DATETIME
	updated DATETIME
	
##Locations

	id INT UNIQUE
	name VARCHAR(50)
	address VARCHAR(255)
	postcode VARCHAR(10) INDEX
	geo_long FLOAT
	geo_lat FLOAT
	telephone VARCHAR(15)
	email VARCHAR(150)
	url VARCHAR(150)
	status SMALLINT {1:Draft, 2:Live, 3:Archive}
	created DATETIME
	updated DATETIME

##LocationSocialAccounts

	id INT UNIQUE
	team_id INT (FK Teams.id)
	social_id INT (FK SocialAccounts.id)
	
##SocialAccounts

	id INT UNIQUE
	service_id INT (FK SocialServices.id)
	url VARCHAR(255)
	status SMALLINT {1:Draft, 2:Live, 3:Archive}
	created DATETIME
	updated DATETIME
	
##SocialAccountServices

	id INT UNIQUE
	name VARCHAR(10)
	
	INSERT INTO SocialAccountServices 
		VALUES  ('Twitter')
				, ('Facebook')
				, ('Instagram')
				, ('Foursquare')
				, ('Google+')
				, ('Snapchat')
				, ('YouTube')