# Generate time-based one time passwords in the browser

[Demo](https://totp.pixelpioneer.surge.sh/)

This page lets you easily generate a time-based one time password (TOTP) entirely in the web browser in case you ever lose access to your phone.

It uses the excellent [otpauth](https://github.com/hectorm/otpauth) package, downloaded from [raw.githubusercontent.com/hectorm/otpauth/master/dist/otpauth.umd.min.js](https://raw.githubusercontent.com/hectorm/otpauth/master/dist/otpauth.umd.min.js).

## Providing parameters in the URL

### Private key

You can provide the key in the URL using the URI fragment or a query parameter, for example: `https://totp.pixelpioneer.surge.sh/#/KEY` or `https://totp.pixelpioneer.surge.sh?key=KEY`

### Additional parameters

You can also pass the token digits, period and algorithm using a query string in the URL, for example: `https://totp.pixelpioneer.surge.sh/?digits=6&period=60&algorithm=SHA256&key=KEY`

See [supported hashing algorithms](https://github.com/hectorm/otpauth#supported-hashing-algorithms) for the complete list.

### Other Resources

* https://www.pommepause.com/2014/10/how-to-extract-your-totp-secrets-from-authy/
* https://github.com/winauth/winauth/issues/545
* https://randomoracle.wordpress.com/2017/02/15/extracting-otp-seeds-from-authy/
* https://gist.github.com/tresni/83b9181588c7393f6853
* https://gist.github.com/Ingramz/14a9c39f8c306a2d43b4
