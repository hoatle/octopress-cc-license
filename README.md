octopress-cc-license
====================

Creative Commons license chooser plugin for octopress as http://creativecommons.org/choose/

Usage
-----

Complete `Installation` and `Configuration` steps, then add the following content into `post.html`
as the example from `source/_layout/post.html`

```
{% if site.cc_license %}
  {% include post/cc_license.html %}
{% endif %}
```


Requirements
------------

- [Octopress](http://octopress.org) version 2.0


Installation
------------

- Copy `source/_include/post/cc_license.html` template
- Copy configuration contents from `_config_cc_license.yml` to `_config.yml`
- Copy contents from `sass/custom/_style_cc_license.scss` to `sass/custom/_style.scss`


Configuration
-------------

- All settings are on `_config.yml`, enable cc_license with: `cc_license: true`

```
# cc license http://creativecommons.org/choose/

# enable cc license?, default: nil means disabled, true to enable
cc_license:

# allow mofiication of works? default: 'yes', options: 'yes', 'no' or 'share'
cc_license_allow_modification: 'yes'

# allow commercial uses of your work? default: true
cc_license_allow_commercial_uses: true

# license jurisdiction? default: International
# //TODO(hoatle): implement cc_license_license_jurisdiction
#cc_license_license_jurisdiction: International

# add metadata? default: nil //TODO(hoatle): implement cc_license_metadata
#cc_license_metadata:

# icon styles? default: 'normal', options: 'normal' or 'compact'.
cc_license_icon: 'normal'

```

- Include `source/_include/post/cc_license.html` to any part of `source/_layout/post.html`.

Sample installation and configuration is at:
https://github.com/teracy-official/blog/commit/4c6feee71b4f2b58d2bed9805580e156093afffe


Contributing
------------

- File issues at https://github.com/hoatle/octopress-cc-license/issues

- Follow Teracy's workflow at http://dev.teracy.org/docs/develop/workflow.html


Discussions
-----------

Join us:

- https://groups.google.com/forum/#!forum/teracy

- https://www.facebook.com/groups/teracy

Get our news:

- https://www.facebook.com/teracy.official

- https://twitter.com/teracy_official


Author and contributors
-----------------------

See more details at `AUTHORS.md` and `CONTRIBUTORS.md` files.


License
-------

BSD License

```
Copyright (c) Teracy, Inc. and individual contributors.
All rights reserved.

Redistribution and use in source and binary forms, with or without modification,
are permitted provided that the following conditions are met:

    1. Redistributions of source code must retain the above copyright notice,
       this list of conditions and the following disclaimer.

    2. Redistributions in binary form must reproduce the above copyright
       notice, this list of conditions and the following disclaimer in the
       documentation and/or other materials provided with the distribution.

    3. Neither the name of Teracy, Inc. nor the names of its contributors may be used
       to endorse or promote products derived from this software without
       specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR
ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```
