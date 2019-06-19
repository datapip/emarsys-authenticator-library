# emarsysauthenticator
Python helper to easily create X-WSSE header for Authentication with Emarsys RESTful API

## Usage
```python
import emarsysauthenticator as ea

# For authentication with Emarsys RESTful API the user name and secret is needed
user_name = 'account_name001'
user_secret = 'abc123def456'

# Create X_WSSE header
xwsse_header = ea.create_xwsse_header(user_name, user_secret)

# Make request
response = requests.request('GET', 'https://api.emarsys.net/api/v2/email', headers=xwsse_header)
```

## Contribution
I am thankful for any feedback and improvements.

## License
This project is licensed under MIT License - see the [LICENSE.md](https://github.com/datapip/emarsysauthenticator/blob/master/LICENSE) file for details 
