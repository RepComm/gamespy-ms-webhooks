
## players
| fieldname | type | modifier |
|--|--|--|
id|int10|PK
sid|int10|MUL
gq_name|varchar255|MUL
gq_team|int11
gq_kills|int11
gq_deaths|int11
gq_score|int11
gq_ping|int11us
lastseen|int11|MUL

## gameserver
| fieldname | type | modifier |
|--|--|--|
id|int11|PK AUTOINC
masterserver|int11
dynamic|int1
challengeok|int1
handshakeok|int1
address|varchar100
port|int11
hostport|int11
protocol|varchar50
type|varchar50
gq_hostname|varchar255
gq_gametype|varchar255
gq_mapname|varchar255
gq_maxplayers|int11
gq_numplayers|int11
team0_name|varchar50
team0_score|int11
team1_name|varchar50
team1_score|int11
gamever|varchar50
session|int11
prevsession|int11
servertype|int1
gamemode|varchar50
localips|varchar255
clientid|int11
netregion|int1
custom|text
lastseen|int11
lastquery|int11

## stats_rounds
| fieldname | type | modifier |
|--|--|--|
id|int11|PK AUTOINC
sid|int11
uid|int11
player|varchar100
auth|varchar255
pid|int11
finishes|int1
deaths|int11
kills|int11
endfaction|varchar20
playerpoints|int11
timePlayed|int11
ctime|int11
dtime|int11
starts|int11
heropoints|int11
livingStreak|int11
rating|int11
mapname|varchar50
winningTeam|varchar20
gameComplete|int1
winningCnt|int11
losingCnt|int11
gametype|varchar50
losingTeam|varchar50
GameMode|int1
timestamp|int11

## stats_servers
| fieldname | type | modifier |
|--|--|--|
stats_servers
id|int11|PK AUTOINC
title|varchar255
desc|text
ip|varchar100
active|int1

## natneg
| fieldname | type | modifier |
|--|--|--|
id|int11|PK AUTOINC
natneg_masterserver|int11
natneg_cookie|int11
natneg_gamename|varchar50
natneg_sequence|int1
natneg_localip|varchar15
natneg_remoteip|varchar15
natneg_remoteport|int11
natneg_clienttype|int1
nagneg_comport|int11
natneg_lastupdate|int11

## masterserver
| fieldname | type | modifier |
|--|--|--|
id|int11|PK AUTOINC
server_name|varchar32
server_address|varchar15
server_port|int11
server_natnegaddress|varchar100
server_natnegport|int11

## serverkeys
| fieldname | type | modifier |
|--|--|--|
id|int11|PK AUTOINC
key_gamename|varchar20
key_key|varchar6
supported|int1

<br/>

Gamespy Login:
## users
| fieldname | type | modifier |
|--|--|--|
id|int11|PK AUTOINC
name|varchar100
password|varchar255
email|varchar50
country|varchar4
session|int11
game|varchar255
status|int1
status_string|varchar255
stats_finishes|int11
stats_deaths|int11
stats_kills|int11
stats_playerpoints|int11
stats_timePlayed|int11
stats_ctime|int11
stats_starts|int11
stats_heropoints|int11
stats_livingStreak|int11
stats_rating|int11
stats_gameComplete|int11
stats_winningCnt|int11
stats_losingCnt|int11
stats_roundsplayed|int11
stats_lastPlayed|int11