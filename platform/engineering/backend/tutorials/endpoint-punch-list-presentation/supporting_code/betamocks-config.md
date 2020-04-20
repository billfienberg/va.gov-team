# betamocks-config

## vets-api/config/betamocks/services\_config.yml

```text
# EVSS
- :name: 'EVSS'
  :base_uri: <%= "#{URI(Settings.evss.url).host}:#{URI(Settings.evss.url).port}" %>
  :endpoints:
  # PCIU email
  - :method: :get
    :path: "/wss-pciu-services-web/rest/pciuServices/v1/emailAddress"
    :file_path: "evss/pciu/email"
    :cache_multiple_responses:
      :uid_location: header
      :uid_locator: 'va_eauth_pnid'
```

## vets-api/config/settings.yml

```text
...

evss:
  mock_pciu: true

...
```

