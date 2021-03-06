# v0.9.1 (01.03.2022)

- [Assume public key encryption unless HMAC is specified](https://gitlab.com/gitlab-org/gitlab-omniauth-openid-connect/-/merge_requests/19)

# v0.9.0 (01.03.2022)

- [Add support for ES[256|384|512|256K] algorithms](https://gitlab.com/gitlab-org/gitlab-omniauth-openid-connect/-/merge_requests/17)

# v0.8.0 (07.16.2021)

- [Add `jwt_secret_base64` option to support binary secrets](https://gitlab.com/gitlab-org/gitlab-omniauth-openid-connect/-/merge_requests/12)

# v0.7.0 (07.16.2021)

- [Add `jwt_secret` option to support Keycloak private key](https://gitlab.com/gitlab-org/gitlab-omniauth-openid-connect/-/merge_requests/10)

# v0.6.0 (07.08.2021)

- [Support verification of HS256-signed JWTs](https://gitlab.com/gitlab-org/gitlab-omniauth-openid-connect/-/merge_requests/8)

# v0.5.0 (05.07.2021)

- [Add email_verified field to info dict](https://gitlab.com/gitlab-org/gitlab-omniauth-openid-connect/-/merge_requests/7)
- [Simplify error handling for decoding individual keys](https://gitlab.com/gitlab-org/gitlab-omniauth-openid-connect/-/merge_requests/6)
- [Always convert client_signing_alg to be a symbol](https://gitlab.com/gitlab-org/gitlab-omniauth-openid-connect/-/merge_requests/5)

# v0.4.0 (04.23.2021)

- [Fetch key from JWKS URI if available](https://gitlab.com/gitlab-org/gitlab-omniauth-openid-connect/-/merge_requests/3)
- [Fix handling of JWT without key ID](https://gitlab.com/gitlab-org/gitlab-omniauth-openid-connect/-/merge_requests/2)
- [Add .gitlab-ci.yml and test with Ruby 3.0](https://gitlab.com/gitlab-org/gitlab-omniauth-openid-connect/-/merge_requests/1)

# v0.3.5 (07.06.2020)

- bugfix: Info from decoded id_token is not exposed into `request.env['omniauth.auth']` [#61](https://github.com/m0n9oose/omniauth_openid_connect/pull/61)
- bugfix: NoMethodError (`undefined method 'count' for #<OpenIDConnect::ResponseObject::IdToken>`) [#60](https://github.com/m0n9oose/omniauth_openid_connect/pull/60)

# v0.3.4 (21.05.2020)

- Try to verify id_token when response_type is code [#44](https://github.com/m0n9oose/omniauth_openid_connect/pull/44)
- Provide more information on error [#49](https://github.com/m0n9oose/omniauth_openid_connect/pull/49)
- Update configuration documentation [#53](https://github.com/m0n9oose/omniauth_openid_connect/pull/53)
- Add documentation about the send_scope_to_token_endpoint config property [#52](https://github.com/m0n9oose/omniauth_openid_connect/pull/52)
- refactor: take uid_field from raw_attributes [#54](https://github.com/m0n9oose/omniauth_openid_connect/pull/54)
- chore(ci): add 2.7, ruby-head and jruby-head [#55](https://github.com/m0n9oose/omniauth_openid_connect/pull/55)

# v0.3.3 (09.11.2019)

- Pass `acr_values` to authorize url [#43](https://github.com/m0n9oose/omniauth_openid_connect/pull/43)
- Add raw info for id token [#42](https://github.com/m0n9oose/omniauth_openid_connect/pull/42)
- Fixed `id_token` verification when `id_token` is not used [#41](https://github.com/m0n9oose/omniauth_openid_connect/pull/41)
- Cast `response_type` to string when checking if it is set in params [#36](https://github.com/m0n9oose/omniauth_openid_connect/pull/36)
- Support both symbol and string version of `response_type` option [#35](https://github.com/m0n9oose/omniauth_openid_connect/pull/35)
- Fix gemspec homepage [#33](https://github.com/m0n9oose/omniauth_openid_connect/pull/33)
- Add support for `response_type` `id_token` [#32](https://github.com/m0n9oose/omniauth_openid_connect/pull/32)

# v0.3.2 (03.08.2019)

- Use response_mode in `authorize_uri` if the option is defined [#30](https://github.com/m0n9oose/omniauth_openid_connect/pull/30)
- Move verification of `id_token` to before accessing tokens [#28](https://github.com/m0n9oose/omniauth_openid_connect/pull/28)
- Update omniauth dependency [#26](https://github.com/m0n9oose/omniauth_openid_connect/pull/26)

# v0.3.1 (08.06.2019)

- Set default OmniAuth name to openid_connect [#23](https://github.com/m0n9oose/omniauth_openid_connect/pull/23)

# v0.3.0 (27.04.2019)

- RP-Initiated Logout phase [#5](https://github.com/m0n9oose/omniauth_openid_connect/pull/5)
- Allows `ui_locales`, `claims_locales` and `login_hint` as request params [#6](https://github.com/m0n9oose/omniauth_openid_connect/pull/6)
- Make uid label configurable [#11](https://github.com/m0n9oose/omniauth_openid_connect/pull/11)
- Allow rails applications to handle state mismatch [#14](https://github.com/m0n9oose/omniauth_openid_connect/pull/14)
- Handle errors when fetching access_token at callback_phase [#17](https://github.com/m0n9oose/omniauth_openid_connect/pull/17)
- Allow state method to receive env [#19](https://github.com/m0n9oose/omniauth_openid_connect/pull/19)

# v0.2.4 (06.01.2019)

- Prompt and login hint [#4](https://github.com/m0n9oose/omniauth_openid_connect/pull/4)
- Bump openid_connect dependency [#9](https://github.com/m0n9oose/omniauth_openid_connect/pull/9)
