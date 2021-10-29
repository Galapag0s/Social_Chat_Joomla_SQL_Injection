# Social_Chat_Joomla_SQL_Injection

The socialchatcore.php file is vulnerable to multiple SQL
injections. These injections affect multiple UPDATE
statements and a SELECT statement. Through the UPDATE
statements, a user could change arbitrary values within the
SocialChat database tables. Through the SELECT statement, a
user can access arbitrary fields within the database. The
following sample payload could be used to extract data in the
form of text via "field_3." POC
PAYLOAD:storico_utente=123)+UNION+SELECT+field_1,field_2,fie
ld_3+FROM+table_name;#&da=from&a=to The developer has
acknowledge the vulnerability and stated that a patch will be
available, despite the fact that the project is no longer in
development.
