# MT4ManagerAPP
MT4 Manager API

Management API, based on the management function of mt4manager, extends the management business.

Functions include:

1》account opening,

Function name：AccOpen

Request method：Post

Parameter：name(Account name).pwd(Password).agroup(Account grouping).leverage（Leverage）.country(country).email(email).group(0:demo 1:real)

Return value：code(0：success,1：failure) msg (success,failure)

2》deposit,

Function name：AccDeposit

Request method：Post

Parameter：login(Account login).amount(amount).comment(comment).expiration(expiration).type(0:Balance+ 1:Balance- 2:Credit+ 3:Credit-).group(0:demo 1:real)

Return value：code(0：success,1：failure) msg (success,failure)

3》modifying lever / group,

Function name：AccSet

Request method：Post

Parameter：login(Account login).type(0:Modify group 1:Modify leverage).value(The corresponding type field is group value or bar value).group(0:demo 1:real)

Return value：code(0：success,1：failure) msg (success,failure)

4》password modification,

Function name：ResetPwd

Request method：Post

Parameter：login(Account login).newpwd(New password).group(0:demo 1:real)

Return value：code(0：success,1：failure) msg (success,failure)

5》account position,

Function name：AccPosition

Request method：Post

Parameter：login(Account login).group(0:demo 1:real)

Return value：code(0：success,1：failure) msg (success,failure)

6》historical records

Function name：HisPosition

Request method：Post

Parameter：login(Account login).from(Start time).to(End time).group(0:demo 1:real)

Return value：code(0：success,1：failure) msg (success,failure)

7》Account information，

Function name：AccInfo

Request method：Post

Parameter：login(Account login).group(0:demo 1:real)

Return value：code(0：success,1：failure) msg (success,failure)

Test the above interface tool: postman ,parameter transfer method form-data.

The function can be realized is not limited to the above introduction, can be customized development, can do source sales, welcome to call to discuss cooperation.
