# Comparing `tmp/psynet-9.4.4.tar.gz` & `tmp/psynet-9.4.5.tar.gz`

## Comparing `psynet-9.4.4.tar` & `psynet-9.4.5.tar`

### file list

```diff
@@ -1,134 +1,132 @@
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 psynet-9.4.4/.flake8
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 psynet-9.4.4/.git-blame-ignore-revs.txt
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 psynet-9.4.4/.gitlab-ci.yml
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 psynet-9.4.4/.jshintrc
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 psynet-9.4.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 psynet-9.4.4/.pylintrc
--rw-r--r--   0        0        0    49168 2020-02-02 00:00:00.000000 psynet-9.4.4/CHANGELOG.md
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 psynet-9.4.4/MANIFEST.in
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psynet-9.4.4/__init__.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 psynet-9.4.4/pytest.ini
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 psynet-9.4.4/setup.cfg
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 psynet-9.4.4/setup.py
--rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 psynet-9.4.4/unity_interface_description.md
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/VERSION
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/__init__.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/audio_mixer.py
--rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/bot.py
--rw-r--r--   0        0        0    23045 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/command_line.py
--rw-r--r--   0        0        0    20168 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/consent.py
--rw-r--r--   0        0        0    18337 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/data.py
--rwxr-xr-x   0        0        0    48778 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/experiment.py
--rw-r--r--   0        0        0    11374 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/field.py
--rw-r--r--   0        0        0    21457 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/graphics.py
--rw-r--r--   0        0        0    16703 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/js_synth.py
--rw-r--r--   0        0        0     9184 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/lucid.py
--rw-r--r--   0        0        0    10805 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/media.py
--rw-r--r--   0        0        0    73963 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/modular_page.py
--rw-r--r--   0        0        0    31849 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/page.py
--rw-r--r--   0        0        0    19464 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/participant.py
--rw-r--r--   0        0        0    68055 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/prescreen.py
--rw-r--r--   0        0        0    11509 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/recruiters.py
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/test.py
--rw-r--r--   0        0        0    78194 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/timeline.py
--rw-r--r--   0        0        0    14736 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/definitions/__init__.py
--rw-r--r--   0        0        0     7449 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/definitions/gold-msi.csv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/demography/__init__.py
--rw-r--r--   0        0        0    30278 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/demography/general.py
--rw-r--r--   0        0        0    22781 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/demography/gmsi.py
--rw-r--r--   0        0        0     5232 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/demography/pei.py
--rw-r--r--   0        0        0    73790 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/resources/favicon.ico
--rw-r--r--   0        0        0    12707 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/resources/logo.png
--rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/resources/logo.svg
--rw-r--r--   0        0        0    18335 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/resources/logo_image_only.png
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/resources/css/consent.css
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/resources/css/dashboard_timeline.css
--rw-r--r--   0        0        0    38441 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/resources/images/princeton-consent.png
--rw-r--r--   0        0        0    18658 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/resources/images/unity_logo.png
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/resources/libraries/Tonejs/LICENSE.md
--rw-r--r--   0        0        0   349554 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/resources/libraries/Tonejs/Tone.js
--rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/resources/libraries/jQuery/jquery-3.6.0.min.js
--rwxr-xr-x   0        0        0       10 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/resources/libraries/jQuery-Knob/.gitignore
--rwxr-xr-x   0        0        0     1082 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/resources/libraries/jQuery-Knob/LICENSE
--rwxr-xr-x   0        0        0     3099 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/resources/libraries/jQuery-Knob/README.md
--rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/resources/libraries/jQuery-Knob/bower.json
--rwxr-xr-x   0        0        0    27045 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/resources/libraries/jQuery-Knob/excanvas.js
--rwxr-xr-x   0        0        0    13014 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/resources/libraries/jQuery-Knob/index.html
--rwxr-xr-x   0        0        0      984 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/resources/libraries/jQuery-Knob/knob.jquery.json
--rwxr-xr-x   0        0        0      589 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/resources/libraries/jQuery-Knob/package.json
--rwxr-xr-x   0        0        0    33487 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/resources/libraries/jQuery-Knob/secretplan.jpg
--rwxr-xr-x   0        0        0    26225 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/resources/libraries/jQuery-Knob/js/jquery.knob.js
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/resources/libraries/js-synthesizer/.gitignore
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/resources/libraries/js-synthesizer/README.txt
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/resources/libraries/js-synthesizer/demo.html
--rw-r--r--   0        0        0     9031 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/resources/libraries/js-synthesizer/instruments.js
--rw-r--r--   0        0        0    11184 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/resources/libraries/js-synthesizer/synthesis.js
--rw-r--r--   0        0        0    14514 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/resources/libraries/platform-1.3.6/platform.min.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/resources/libraries/raphael-2.3.0/.eslintrc.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/resources/libraries/raphael-2.3.0/.gitignore
--rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/resources/libraries/raphael-2.3.0/README.md
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/resources/libraries/raphael-2.3.0/license.txt
--rw-r--r--   0        0        0    93167 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/resources/libraries/raphael-2.3.0/raphael.min.js
--rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/resources/scripts/dashboard_timeline.js
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/resources/scripts/prepare_docker_image.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/__init__.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/abort_not_possible.html
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/abort_possible.html
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/ad.html
--rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/consent.html
--rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/dashboard_timeline.html
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/exit_recruiter_lucid.html
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/final-page-bonuses.html
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/final-page-rejected-consent.html
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/final-page-successful.html
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/final-page-unsuccessful.html
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/info-page.html
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/macros.html
--rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/mturk_error.html
--rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/participant.html
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/psynet_layout.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/questions.html
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/resume.html
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/start.html
--rw-r--r--   0        0        0    67246 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/timeline-page.html
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/unity-debug-page.html
--rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/unity-page.html
--rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/wait-page.html
--rw-r--r--   0        0        0     5328 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/consents/audiovisual_consent.html
--rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/consents/cap-recruiter_audiovisual_consent.html
--rw-r--r--   0        0        0     3558 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/consents/cap-recruiter_standard_consent.html
--rw-r--r--   0        0        0     8508 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/consents/database_consent.html
--rw-r--r--   0        0        0     9239 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/consents/main_consent.html
--rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/consents/mturk_audiovisual_consent.html
--rw-r--r--   0        0        0    11039 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/consents/mturk_standard_consent.html
--rw-r--r--   0        0        0     3921 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/consents/open_science_consent.html
--rw-r--r--   0        0        0     8405 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/consents/princeton_cap_recruiter_consent.html
--rw-r--r--   0        0        0     8041 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/consents/princeton_consent.html
--rw-r--r--   0        0        0     8792 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/consents/voluntary_with_no_compensation_consent.html
--rw-r--r--   0        0        0    62854 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/macros/control.html
--rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/macros/graphics.html
--rw-r--r--   0        0        0    10625 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/macros/prompt.html
--rw-r--r--   0        0        0   194322 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/macros/control/RecordRTC.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/macros/control/__init__.py
--rw-r--r--   0        0        0   199443 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/macros/control/adapter.js
--rw-r--r--   0        0        0     9070 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/macros/control/audio_meter.js
--rw-r--r--   0        0        0    13051 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/templates/macros/control/recorder.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/trial/__init__.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/trial/audio.py
--rw-r--r--   0        0        0    15679 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/trial/audio_gibbs.py
--rw-r--r--   0        0        0    52506 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/trial/chain.py
--rw-r--r--   0        0        0    30793 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/trial/dense.py
--rw-r--r--   0        0        0    12498 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/trial/gibbs.py
--rw-r--r--   0        0        0    15741 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/trial/graph.py
--rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/trial/imitation_chain.py
--rw-r--r--   0        0        0    88441 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/trial/main.py
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/trial/mcmcp.py
--rw-r--r--   0        0        0     7742 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/trial/record.py
--rw-r--r--   0        0        0    57654 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/trial/static.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 psynet-9.4.4/psynet/trial/video.py
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 psynet-9.4.4/.gitignore
--rwxr-xr-x   0        0        0     1126 2020-02-02 00:00:00.000000 psynet-9.4.4/LICENSE
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 psynet-9.4.4/README.md
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 psynet-9.4.4/pyproject.toml
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 psynet-9.4.4/PKG-INFO
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 psynet-9.4.5/.flake8
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 psynet-9.4.5/.git-blame-ignore-revs.txt
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 psynet-9.4.5/.gitlab-ci.yml
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 psynet-9.4.5/.jshintrc
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 psynet-9.4.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 psynet-9.4.5/.pylintrc
+-rw-r--r--   0        0        0    49767 2020-02-02 00:00:00.000000 psynet-9.4.5/CHANGELOG.md
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 psynet-9.4.5/MANIFEST.in
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psynet-9.4.5/__init__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 psynet-9.4.5/pytest.ini
+-rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 psynet-9.4.5/unity_interface_description.md
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/VERSION
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/__init__.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/audio_mixer.py
+-rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/bot.py
+-rw-r--r--   0        0        0    23045 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/command_line.py
+-rw-r--r--   0        0        0    20168 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/consent.py
+-rw-r--r--   0        0        0    18337 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/data.py
+-rwxr-xr-x   0        0        0    48778 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/experiment.py
+-rw-r--r--   0        0        0    11374 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/field.py
+-rw-r--r--   0        0        0    21457 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/graphics.py
+-rw-r--r--   0        0        0    16703 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/js_synth.py
+-rw-r--r--   0        0        0     9184 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/lucid.py
+-rw-r--r--   0        0        0    10805 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/media.py
+-rw-r--r--   0        0        0    73963 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/modular_page.py
+-rw-r--r--   0        0        0    31849 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/page.py
+-rw-r--r--   0        0        0    19464 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/participant.py
+-rw-r--r--   0        0        0    68055 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/prescreen.py
+-rw-r--r--   0        0        0    11509 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/recruiters.py
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/test.py
+-rw-r--r--   0        0        0    78194 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/timeline.py
+-rw-r--r--   0        0        0    14736 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/definitions/__init__.py
+-rw-r--r--   0        0        0     7449 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/definitions/gold-msi.csv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/demography/__init__.py
+-rw-r--r--   0        0        0    37278 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/demography/general.py
+-rw-r--r--   0        0        0    22781 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/demography/gmsi.py
+-rw-r--r--   0        0        0     5232 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/demography/pei.py
+-rw-r--r--   0        0        0    73790 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/favicon.ico
+-rw-r--r--   0        0        0    12707 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/logo.png
+-rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/logo.svg
+-rw-r--r--   0        0        0    18335 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/logo_image_only.png
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/css/consent.css
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/css/dashboard_timeline.css
+-rw-r--r--   0        0        0    38441 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/images/princeton-consent.png
+-rw-r--r--   0        0        0    18658 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/images/unity_logo.png
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/Tonejs/LICENSE.md
+-rw-r--r--   0        0        0   349554 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/Tonejs/Tone.js
+-rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/jQuery/jquery-3.6.0.min.js
+-rwxr-xr-x   0        0        0       10 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/.gitignore
+-rwxr-xr-x   0        0        0     1082 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/LICENSE
+-rwxr-xr-x   0        0        0     3099 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/README.md
+-rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/bower.json
+-rwxr-xr-x   0        0        0    27045 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/excanvas.js
+-rwxr-xr-x   0        0        0    13014 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/index.html
+-rwxr-xr-x   0        0        0      984 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/knob.jquery.json
+-rwxr-xr-x   0        0        0      589 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/package.json
+-rwxr-xr-x   0        0        0    33487 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/secretplan.jpg
+-rwxr-xr-x   0        0        0    26225 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/js/jquery.knob.js
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/js-synthesizer/.gitignore
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/js-synthesizer/README.txt
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/js-synthesizer/demo.html
+-rw-r--r--   0        0        0     9031 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/js-synthesizer/instruments.js
+-rw-r--r--   0        0        0    11184 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/js-synthesizer/synthesis.js
+-rw-r--r--   0        0        0    14514 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/platform-1.3.6/platform.min.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/raphael-2.3.0/.eslintrc.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/raphael-2.3.0/.gitignore
+-rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/raphael-2.3.0/README.md
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/raphael-2.3.0/license.txt
+-rw-r--r--   0        0        0    93167 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/libraries/raphael-2.3.0/raphael.min.js
+-rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/scripts/dashboard_timeline.js
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/resources/scripts/prepare_docker_image.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/__init__.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/abort_not_possible.html
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/abort_possible.html
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/ad.html
+-rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/consent.html
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/dashboard_timeline.html
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/exit_recruiter_lucid.html
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/final-page-bonuses.html
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/final-page-rejected-consent.html
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/final-page-successful.html
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/final-page-unsuccessful.html
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/info-page.html
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/macros.html
+-rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/mturk_error.html
+-rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/participant.html
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/psynet_layout.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/questions.html
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/resume.html
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/start.html
+-rw-r--r--   0        0        0    67246 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/timeline-page.html
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/unity-debug-page.html
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/unity-page.html
+-rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/wait-page.html
+-rw-r--r--   0        0        0     5328 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/consents/audiovisual_consent.html
+-rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/consents/cap-recruiter_audiovisual_consent.html
+-rw-r--r--   0        0        0     3558 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/consents/cap-recruiter_standard_consent.html
+-rw-r--r--   0        0        0     8508 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/consents/database_consent.html
+-rw-r--r--   0        0        0     9239 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/consents/main_consent.html
+-rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/consents/mturk_audiovisual_consent.html
+-rw-r--r--   0        0        0    11039 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/consents/mturk_standard_consent.html
+-rw-r--r--   0        0        0     3921 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/consents/open_science_consent.html
+-rw-r--r--   0        0        0     8405 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/consents/princeton_cap_recruiter_consent.html
+-rw-r--r--   0        0        0     8041 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/consents/princeton_consent.html
+-rw-r--r--   0        0        0     8792 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/consents/voluntary_with_no_compensation_consent.html
+-rw-r--r--   0        0        0    62854 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/macros/control.html
+-rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/macros/graphics.html
+-rw-r--r--   0        0        0    10625 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/macros/prompt.html
+-rw-r--r--   0        0        0   194322 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/macros/control/RecordRTC.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/macros/control/__init__.py
+-rw-r--r--   0        0        0   199443 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/macros/control/adapter.js
+-rw-r--r--   0        0        0     9070 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/macros/control/audio_meter.js
+-rw-r--r--   0        0        0    13051 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/templates/macros/control/recorder.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/trial/__init__.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/trial/audio.py
+-rw-r--r--   0        0        0    15679 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/trial/audio_gibbs.py
+-rw-r--r--   0        0        0    52506 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/trial/chain.py
+-rw-r--r--   0        0        0    30793 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/trial/dense.py
+-rw-r--r--   0        0        0    12498 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/trial/gibbs.py
+-rw-r--r--   0        0        0    15741 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/trial/graph.py
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/trial/imitation_chain.py
+-rw-r--r--   0        0        0    88618 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/trial/main.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/trial/mcmcp.py
+-rw-r--r--   0        0        0     7742 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/trial/record.py
+-rw-r--r--   0        0        0    57654 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/trial/static.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 psynet-9.4.5/psynet/trial/video.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 psynet-9.4.5/.gitignore
+-rwxr-xr-x   0        0        0     1126 2020-02-02 00:00:00.000000 psynet-9.4.5/LICENSE
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 psynet-9.4.5/README.md
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 psynet-9.4.5/pyproject.toml
+-rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 psynet-9.4.5/PKG-INFO
```

### Comparing `psynet-9.4.4/.gitlab-ci.yml` & `psynet-9.4.5/.gitlab-ci.yml`

 * *Files 10% similar despite different names*

```diff
@@ -22,29 +22,29 @@
 
 before_script:
 # General setup
   - apt update
   - apt -f -y install curl redis-server unzip
   - service redis-server start
   - curl https://cli-assets.heroku.com/install.sh | sh
-  - wget -O chrome.deb http://dl.google.com/linux/chrome/deb/pool/main/g/google-chrome-stable/google-chrome-stable_101.0.4951.64-1_amd64.deb
-  - wget -O chrome-driver.zip https://chromedriver.storage.googleapis.com/101.0.4951.41/chromedriver_linux64.zip
+  - wget -O chrome.deb http://dl.google.com/linux/chrome/deb/pool/main/g/google-chrome-stable/google-chrome-stable_109.0.5414.74-1_amd64.deb
+  - wget -O chrome-driver.zip https://chromedriver.storage.googleapis.com/109.0.5414.74/chromedriver_linux64.zip
   - apt -f -y install ./chrome.deb
   - unzip chrome-driver.zip chromedriver -d /usr/local/bin/
   - pip install "git+https://gitlab+deploy-token-478431:98jnkW1yq_AYWLYpRNtN@gitlab.com/computational-audition-lab/melody/melody-experiments@master#egg=melody_experiments[extract]"
   - pip install pytest-test-groups
   - export HEADLESS=TRUE
 # Install and setup PostgreSQL
   - apt install -y postgresql postgresql-contrib libpq-dev
   - service postgresql start
   - runuser -l postgres -c 'echo -e "dallinger\ndallinger" | createuser -P -e dallinger'
   - chown postgres:postgres postgres_setup.sql
   - runuser -l postgres -c 'psql -c "\i /builds/PsyNetDev/PsyNet/postgres_setup.sql"'
 # Install Dallinger
-  - git clone --branch v9.4.2 https://github.com/Dallinger/Dallinger.git /tmp/dallinger
+  - git clone --branch v9.6.0 https://github.com/Dallinger/Dallinger.git /tmp/dallinger
   - pip install -r /tmp/dallinger/dev-requirements.txt
   - pip install -e '/tmp/dallinger[data]'
 # Install PsyNet
   - pip install -e '.[dev]'
 
 tests:
   parallel: 5
```

### Comparing `psynet-9.4.4/CHANGELOG.md` & `psynet-9.4.5/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,22 @@
 # CHANGELOG
 
+# [9.4.5] Released on 2023-04-24
+
+#### Fixed
+- Added a random key to Unity assets to avoid caching in the browser (author: Pol van Rijn, reviewer: Frank Höger).
+
+#### Added
+- Added `BigFiveQuestionnaire` and `AltruismQuestionnaire` (author: Pol van Rijn, reviewer: Frank Höger).
+
+#### Updated
+- Completed migration to `pyproject.toml`, incl. removal of `setup.cfg` and `setup.py` (author: Frank Höger).
+- Updated docs for bumpversion removal (author: Frank Höger).
+- Updated `Dallinger` to `v9.6.0`. See the complete release notes at https://github.com/Dallinger/Dallinger/releases/tag/v9.6.0.
+
 # [9.4.4] Released on 2023-02-14
 
 #### Updated
 - Updated `Dallinger` to `v9.4.2` which contains bugfixes and a fix for `pyopenssl` not being updated to the latest version. See the complete release notes at https://github.com/Dallinger/Dallinger/releases/tag/v9.4.2.
 
 # [9.4.3] Released on 2023-01-25
```

### Comparing `psynet-9.4.4/MANIFEST.in` & `psynet-9.4.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/unity_interface_description.md` & `psynet-9.4.5/unity_interface_description.md`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/audio_mixer.py` & `psynet-9.4.5/psynet/audio_mixer.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/bot.py` & `psynet-9.4.5/psynet/bot.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/command_line.py` & `psynet-9.4.5/psynet/command_line.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/consent.py` & `psynet-9.4.5/psynet/consent.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/data.py` & `psynet-9.4.5/psynet/data.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/experiment.py` & `psynet-9.4.5/psynet/experiment.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/field.py` & `psynet-9.4.5/psynet/field.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/graphics.py` & `psynet-9.4.5/psynet/graphics.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/js_synth.py` & `psynet-9.4.5/psynet/js_synth.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/lucid.py` & `psynet-9.4.5/psynet/lucid.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/media.py` & `psynet-9.4.5/psynet/media.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/modular_page.py` & `psynet-9.4.5/psynet/modular_page.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/page.py` & `psynet-9.4.5/psynet/page.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/participant.py` & `psynet-9.4.5/psynet/participant.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/prescreen.py` & `psynet-9.4.5/psynet/prescreen.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/recruiters.py` & `psynet-9.4.5/psynet/recruiters.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/test.py` & `psynet-9.4.5/psynet/test.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/timeline.py` & `psynet-9.4.5/psynet/timeline.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/utils.py` & `psynet-9.4.5/psynet/utils.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/definitions/gold-msi.csv` & `psynet-9.4.5/psynet/definitions/gold-msi.csv`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/demography/general.py` & `psynet-9.4.5/psynet/demography/general.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,21 @@
+import numpy as np
+from markupsafe import Markup
+
 from psynet.modular_page import (
     DropdownControl,
     ModularPage,
     NumberControl,
     PushButtonControl,
     RadioButtonControl,
     TextControl,
 )
+from psynet.page import InfoPage
 from psynet.timeline import FailedValidation, Module, conditional, join
+from psynet.trial.static import StaticTrial, StaticTrialMaker, StimulusSet, StimulusSpec
 from psynet.utils import get_logger
 
 logger = get_logger()
 
 
 class BasicDemography(Module):
     def __init__(
@@ -588,14 +593,254 @@
             self.label,
             self.prompt,
             control=TextControl(),
             time_estimate=self.time_estimate,
         )
 
 
+class PersonalityTrial(StaticTrial):
+    time_estimate = 5
+
+    def show_trial(self, experiment, participant):
+        trial_maker = experiment.timeline.get_trial_maker(self.trial_maker_id)
+        answer_options = trial_maker.get_answer_options()
+        choices = list(range(1, len(answer_options) + 1))
+
+        return ModularPage(
+            trial_maker.get_default_label() + "_trial",
+            Markup(
+                trial_maker.get_question_prefix()
+                + " <strong>"
+                + self.definition["option"]
+                + "</strong>"
+            ),
+            PushButtonControl(
+                choices,
+                answer_options,
+                arrange_vertically=True,
+                style="min-width: 10px; margin: 10px",
+            ),
+            time_estimate=self.time_estimate,
+        )
+
+
+class PersonalityTrialMaker(StaticTrialMaker):
+    @staticmethod
+    def get_default_label():
+        raise NotImplementedError
+
+    @staticmethod
+    def get_questions():
+        raise NotImplementedError
+
+    @staticmethod
+    def get_question_prefix():
+        raise NotImplementedError
+
+    @staticmethod
+    def get_answer_options():
+        raise NotImplementedError
+
+
+class PersonalityQuestionnaire(Module):
+    """
+    This is a template for personality questionnaires.
+
+    Parameters
+    ----------
+
+    label : string, optional
+    """
+
+    def __init__(
+        self,
+        label=None,
+        check_performance_at_end=False,
+    ):
+        if label is None:
+            label = self.get_default_label()
+        self.label = label
+
+        trial_maker_class = self.get_trial_maker_class()
+        questions = trial_maker_class.get_questions()
+        self.elts = join(
+            self.instruction_page(),
+            trial_maker_class(
+                id_=self.get_default_label() + "_trial_maker",
+                trial_class=self.get_trial_class(),
+                phase="screening",
+                stimulus_set=self.get_stimulus_set(questions),
+                max_trials_per_block=len(questions),
+                check_performance_at_end=check_performance_at_end,
+            ),
+        )
+        super().__init__(self.label, self.elts)
+
+    def instruction_page(self):
+        return InfoPage(
+            "We now have a few questions about you",
+            time_estimate=5,
+        )
+
+    @staticmethod
+    def get_trial_maker_class():
+        return PersonalityTrialMaker
+
+    def get_default_label(self):
+        return self.get_trial_maker_class().get_default_label()
+
+    @staticmethod
+    def get_trial_class():
+        return PersonalityTrial
+
+    def get_stimulus_set(self, answer_options):
+        return StimulusSet(
+            self.get_default_label() + "_questions",
+            [
+                StimulusSpec(
+                    definition={"option": option},
+                    phase="screening",
+                )
+                for option in answer_options
+            ],
+        )
+
+
+class BigFiveTrialMaker(PersonalityTrialMaker):
+    @staticmethod
+    def get_default_label():
+        return "big_five_questionnaire"
+
+    @staticmethod
+    def get_questions():
+        return [
+            "is reserved",
+            "is generally trusting",
+            "tends to be lazy",
+            "is relaxed, handles stress well",
+            "has few artistic interests",
+            "is outgoing, sociable",
+            "tends to find fault with others",
+            "does a thorough job",
+            "gets nervous easily",
+            "has an active imagination",
+        ]
+
+    @staticmethod
+    def get_question_prefix():
+        return "I see myself as someone who"
+
+    @staticmethod
+    def get_answer_options():
+        return [
+            "1 (Disagree strongly)",
+            "2 (Disagree a little)",
+            "3 (Neither agree nor disagree)",
+            "4 (Agree a little)",
+            "5 (Agree strongly)",
+        ]
+
+    def performance_check(self, experiment, participant, participant_trials):
+        def flip_scale(score):
+            return 6 - score
+
+        def mean(scores):
+            return float(np.mean(scores))
+
+        responses = {
+            trial.definition["option"]: int(trial.answer)
+            for trial in participant_trials
+        }
+        score = {
+            "Extraversion": mean(
+                [
+                    flip_scale(responses["is reserved"]),
+                    responses["has few artistic interests"],
+                ]
+            ),
+            "Agreeableness": mean(
+                [
+                    responses["is generally trusting"],
+                    flip_scale(responses["tends to find fault with others"]),
+                ]
+            ),
+            "Conscientiousness": mean(
+                [
+                    flip_scale(responses["tends to be lazy"]),
+                    responses["does a thorough job"],
+                ]
+            ),
+            "Neuroticism": mean(
+                [
+                    flip_scale(responses["is relaxed, handles stress well"]),
+                    responses["gets nervous easily"],
+                ]
+            ),
+            "Openness": mean(
+                [
+                    flip_scale(responses["has few artistic interests"]),
+                    responses["has an active imagination"],
+                ]
+            ),
+        }
+        return {"score": score, "passed": True}
+
+
+class BigFiveQuestionnaire(PersonalityQuestionnaire):
+    def __init__(
+        self,
+        label=None,
+        check_performance_at_end=True,
+    ):
+        super().__init__(label, check_performance_at_end)
+
+    @staticmethod
+    def get_trial_maker_class():
+        return BigFiveTrialMaker
+
+
+class AltruismTrialMaker(PersonalityTrialMaker):
+    @staticmethod
+    def get_default_label():
+        return "altruism_questionnaire"
+
+    @staticmethod
+    def get_questions():
+        return [
+            "given money to a charity",
+            "donated goods or clothes to a charity",
+            "done volunteer work for a charity",
+            "helped carry a stranger’s belongings",
+            "made change for someone I did not know",
+            "helped an acquaintance to move houses",
+            "let a neighbor I did not know well borrow an item of some value to me",
+            "offered to help a disabled or elderly stranger across a street",
+            "offered my seat to a stranger who was standing",
+        ]
+
+    @staticmethod
+    def get_question_prefix():
+        return "I have"
+
+    @staticmethod
+    def get_answer_options():
+        return [
+            "1 Never",
+            "2 Rarely",
+            "3 Sometimes",
+            "4 Frequently",
+            "5 Always",
+        ]
+
+
+class AltruismQuestionnaire(PersonalityQuestionnaire):
+    def get_trial_maker_class(self):
+        return AltruismTrialMaker
+
+
 def countries():
     """
     List compiled using the pycountry package v20.7.3 with
     ``
     sorted([(lang.alpha_2, lang.name) for lang in pycountry.countries
         if hasattr(lang, 'alpha_2')], key=lambda country: country[1])
     ``
```

### Comparing `psynet-9.4.4/psynet/demography/gmsi.py` & `psynet-9.4.5/psynet/demography/gmsi.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/demography/pei.py` & `psynet-9.4.5/psynet/demography/pei.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/resources/favicon.ico` & `psynet-9.4.5/psynet/resources/favicon.ico`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/resources/logo.png` & `psynet-9.4.5/psynet/resources/logo.png`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/resources/logo.svg` & `psynet-9.4.5/psynet/resources/logo.svg`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/resources/logo_image_only.png` & `psynet-9.4.5/psynet/resources/logo_image_only.png`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/resources/css/dashboard_timeline.css` & `psynet-9.4.5/psynet/resources/css/dashboard_timeline.css`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/resources/images/princeton-consent.png` & `psynet-9.4.5/psynet/resources/images/princeton-consent.png`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/resources/images/unity_logo.png` & `psynet-9.4.5/psynet/resources/images/unity_logo.png`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/resources/libraries/Tonejs/LICENSE.md` & `psynet-9.4.5/psynet/resources/libraries/Tonejs/LICENSE.md`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/resources/libraries/Tonejs/Tone.js` & `psynet-9.4.5/psynet/resources/libraries/Tonejs/Tone.js`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/resources/libraries/jQuery/jquery-3.6.0.min.js` & `psynet-9.4.5/psynet/resources/libraries/jQuery/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/resources/libraries/jQuery-Knob/LICENSE` & `psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/LICENSE`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/resources/libraries/jQuery-Knob/README.md` & `psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/README.md`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/resources/libraries/jQuery-Knob/excanvas.js` & `psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/excanvas.js`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/resources/libraries/jQuery-Knob/index.html` & `psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/index.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/resources/libraries/jQuery-Knob/knob.jquery.json` & `psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/knob.jquery.json`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/resources/libraries/jQuery-Knob/package.json` & `psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/package.json`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/resources/libraries/jQuery-Knob/secretplan.jpg` & `psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/secretplan.jpg`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/resources/libraries/jQuery-Knob/js/jquery.knob.js` & `psynet-9.4.5/psynet/resources/libraries/jQuery-Knob/js/jquery.knob.js`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/resources/libraries/js-synthesizer/README.txt` & `psynet-9.4.5/psynet/resources/libraries/js-synthesizer/README.txt`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/resources/libraries/js-synthesizer/demo.html` & `psynet-9.4.5/psynet/resources/libraries/js-synthesizer/demo.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/resources/libraries/js-synthesizer/instruments.js` & `psynet-9.4.5/psynet/resources/libraries/js-synthesizer/instruments.js`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/resources/libraries/js-synthesizer/synthesis.js` & `psynet-9.4.5/psynet/resources/libraries/js-synthesizer/synthesis.js`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/resources/libraries/platform-1.3.6/platform.min.js` & `psynet-9.4.5/psynet/resources/libraries/platform-1.3.6/platform.min.js`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/resources/libraries/raphael-2.3.0/README.md` & `psynet-9.4.5/psynet/resources/libraries/raphael-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/resources/libraries/raphael-2.3.0/license.txt` & `psynet-9.4.5/psynet/resources/libraries/raphael-2.3.0/license.txt`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/resources/libraries/raphael-2.3.0/raphael.min.js` & `psynet-9.4.5/psynet/resources/libraries/raphael-2.3.0/raphael.min.js`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/resources/scripts/dashboard_timeline.js` & `psynet-9.4.5/psynet/resources/scripts/dashboard_timeline.js`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/resources/scripts/prepare_docker_image.sh` & `psynet-9.4.5/psynet/resources/scripts/prepare_docker_image.sh`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/templates/abort_not_possible.html` & `psynet-9.4.5/psynet/templates/abort_not_possible.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/templates/abort_possible.html` & `psynet-9.4.5/psynet/templates/abort_possible.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/templates/ad.html` & `psynet-9.4.5/psynet/templates/ad.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/templates/consent.html` & `psynet-9.4.5/psynet/templates/consent.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/templates/dashboard_timeline.html` & `psynet-9.4.5/psynet/templates/dashboard_timeline.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/templates/exit_recruiter_lucid.html` & `psynet-9.4.5/psynet/templates/exit_recruiter_lucid.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/templates/final-page-unsuccessful.html` & `psynet-9.4.5/psynet/templates/final-page-unsuccessful.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/templates/mturk_error.html` & `psynet-9.4.5/psynet/templates/mturk_error.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/templates/participant.html` & `psynet-9.4.5/psynet/templates/participant.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/templates/psynet_layout.html` & `psynet-9.4.5/psynet/templates/psynet_layout.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/templates/resume.html` & `psynet-9.4.5/psynet/templates/resume.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/templates/start.html` & `psynet-9.4.5/psynet/templates/start.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/templates/timeline-page.html` & `psynet-9.4.5/psynet/templates/timeline-page.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/templates/unity-debug-page.html` & `psynet-9.4.5/psynet/templates/unity-debug-page.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/templates/unity-page.html` & `psynet-9.4.5/psynet/templates/unity-page.html`

 * *Files 12% similar despite different names*

```diff
@@ -30,20 +30,21 @@
       <div id="unity-footer">
         <div id="unity-webgl-logo"></div>
         <div id="unity-fullscreen-button"></div>
         <div id="unity-build-title">{{ title }}</div>
       </div>
     </div>
     <script>
+      let randomKey = Math.random().toString(36).substring(7);  // random key to prevent caching
       let buildUrl = "{{ resources }}/scripts/Build";
-      let loaderUrl = "{{ resources }}/scripts/Build/WebGL.loader.js";
+      let loaderUrl = buildUrl + "/WebGL.loader.js?random=" + randomKey;
       let config = {
-        dataUrl: buildUrl + "/WebGL.data",
-        frameworkUrl: buildUrl + "/WebGL.framework.js",
-        codeUrl: buildUrl + "/WebGL.wasm",
+        dataUrl: buildUrl + "/WebGL.data?random=" + randomKey,
+        frameworkUrl: buildUrl + "/WebGL.framework.js?random=" + randomKey,
+        codeUrl: buildUrl + "/WebGL.wasm?random=" + randomKey,
       };
 
       let container = document.querySelector("#unity-container");
       let canvas = document.querySelector("#unity-canvas");
       let loadingBar = document.querySelector("#unity-loading-bar");
       let progressBarFull = document.querySelector("#unity-progress-bar-full");
       let fullscreenButton = document.querySelector("#unity-fullscreen-button");
```

### Comparing `psynet-9.4.4/psynet/templates/wait-page.html` & `psynet-9.4.5/psynet/templates/wait-page.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/templates/consents/audiovisual_consent.html` & `psynet-9.4.5/psynet/templates/consents/audiovisual_consent.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/templates/consents/cap-recruiter_audiovisual_consent.html` & `psynet-9.4.5/psynet/templates/consents/cap-recruiter_audiovisual_consent.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/templates/consents/cap-recruiter_standard_consent.html` & `psynet-9.4.5/psynet/templates/consents/cap-recruiter_standard_consent.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/templates/consents/database_consent.html` & `psynet-9.4.5/psynet/templates/consents/database_consent.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/templates/consents/main_consent.html` & `psynet-9.4.5/psynet/templates/consents/main_consent.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/templates/consents/mturk_audiovisual_consent.html` & `psynet-9.4.5/psynet/templates/consents/mturk_audiovisual_consent.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/templates/consents/mturk_standard_consent.html` & `psynet-9.4.5/psynet/templates/consents/mturk_standard_consent.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/templates/consents/open_science_consent.html` & `psynet-9.4.5/psynet/templates/consents/open_science_consent.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/templates/consents/princeton_cap_recruiter_consent.html` & `psynet-9.4.5/psynet/templates/consents/princeton_cap_recruiter_consent.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/templates/consents/princeton_consent.html` & `psynet-9.4.5/psynet/templates/consents/princeton_consent.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/templates/consents/voluntary_with_no_compensation_consent.html` & `psynet-9.4.5/psynet/templates/consents/voluntary_with_no_compensation_consent.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/templates/macros/control.html` & `psynet-9.4.5/psynet/templates/macros/control.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/templates/macros/graphics.html` & `psynet-9.4.5/psynet/templates/macros/graphics.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/templates/macros/prompt.html` & `psynet-9.4.5/psynet/templates/macros/prompt.html`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/templates/macros/control/RecordRTC.js` & `psynet-9.4.5/psynet/templates/macros/control/RecordRTC.js`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/templates/macros/control/adapter.js` & `psynet-9.4.5/psynet/templates/macros/control/adapter.js`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/templates/macros/control/audio_meter.js` & `psynet-9.4.5/psynet/templates/macros/control/audio_meter.js`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/templates/macros/control/recorder.js` & `psynet-9.4.5/psynet/templates/macros/control/recorder.js`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/trial/audio.py` & `psynet-9.4.5/psynet/trial/audio.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/trial/audio_gibbs.py` & `psynet-9.4.5/psynet/trial/audio_gibbs.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/trial/chain.py` & `psynet-9.4.5/psynet/trial/chain.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/trial/dense.py` & `psynet-9.4.5/psynet/trial/dense.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/trial/gibbs.py` & `psynet-9.4.5/psynet/trial/gibbs.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/trial/graph.py` & `psynet-9.4.5/psynet/trial/graph.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/trial/imitation_chain.py` & `psynet-9.4.5/psynet/trial/imitation_chain.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/trial/main.py` & `psynet-9.4.5/psynet/trial/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import dallinger.nodes
 from dallinger import db
 from dallinger.db import redis_conn
 from dallinger.models import Info, Network, Node
 from dominate import tags
 from flask import Markup
 from rq import Queue
-from sqlalchemy import Column, String
+from sqlalchemy import Boolean, Column, String
 from sqlalchemy.dialects.postgresql import JSONB
 from sqlalchemy.ext.declarative import declared_attr
 from sqlalchemy.ext.hybrid import hybrid_property
 from sqlalchemy.sql.expression import cast
 
 from ..data import SQLMixinDallinger
 from ..field import (
@@ -396,15 +396,21 @@
         **SQLMixinDallinger.__extra_vars__.copy(),
         **AsyncProcessOwner.__extra_vars__.copy(),
         **HasDefinition.__extra_vars__.copy(),
     }
 
     # Properties ###
     participant_id = claim_field("participant_id", __extra_vars__, int)
-    complete = claim_field("complete", __extra_vars__, bool)
+
+    @declared_attr
+    def complete(cls):
+        # Dallinger v9.6.0 adds an Info.complete column.
+        # The following code inherits that column if it exists.
+        return cls.__table__.c.get("complete", Column(Boolean))
+
     finalized = claim_field("finalized", __extra_vars__, bool)
     is_repeat_trial = claim_field("is_repeat_trial", __extra_vars__, bool)
     score = claim_field("score", __extra_vars__, float)
     bonus = claim_field("bonus", __extra_vars__, float)
     parent_trial_id = claim_field("parent_trial_id", __extra_vars__, int)
     answer = claim_field("answer", __extra_vars__)
     propagate_failure = claim_field("propagate_failure", __extra_vars__, bool)
```

### Comparing `psynet-9.4.4/psynet/trial/mcmcp.py` & `psynet-9.4.5/psynet/trial/mcmcp.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/trial/record.py` & `psynet-9.4.5/psynet/trial/record.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/trial/static.py` & `psynet-9.4.5/psynet/trial/static.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/psynet/trial/video.py` & `psynet-9.4.5/psynet/trial/video.py`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/.gitignore` & `psynet-9.4.5/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -134,14 +134,15 @@
 # RStudio project files
 **.Rproj.user/
 **.Rproj.user*
 **.Rproj
 **.Rhistory
 
 # Other
+.deploy
 .DS_Store
 .vscode/settings.json
 psynet/nips/colour/data/colmcmcp-data.zip
 psynet/nips/colour/data/coltest-data.zip
 psynet/nips/ganspace/snapshots/ganspace-code.zip
 psynet/nips/ganspace/.vscode/settings.json
 .Rproj.user
```

### Comparing `psynet-9.4.4/LICENSE` & `psynet-9.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/README.md` & `psynet-9.4.5/README.md`

 * *Files identical despite different names*

### Comparing `psynet-9.4.4/pyproject.toml` & `psynet-9.4.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,73 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "psynet"
-version = "9.4.4"
+version = "9.4.5"
 authors = [
   { name="Peter Harrison", email="pmch2@cam.ac.uk" },
   { name="Frank Höger", email="frank.hoeger@ae.mpg.de" },
   { name="Pol van Rijn", email="pol.van-rijn@ae.mpg.de" },
   { name="Raja Marjieh", email="raja.marjieh@princeton.edu" },
   { name="Nori Jacoby", email="nori.jacoby@ae.mpg.de" }
 ]
+maintainers = [
+  {name = "Peter Harrison", email = "pmch2@cam.ac.uk"}
+]
+license = {file = "LICENSE"}
 description = "PsyNet – The online human behaviour lab of the future"
+keywords = ["psychology", "experiments", "online", "networks"]
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
+    "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
+    "Framework :: Flask",
     "Operating System :: OS Independent",
+    "License :: OSI Approved :: MIT License",
+    "Intended Audience :: Science/Research",
 ]
 dependencies = [
+    "dallinger>=9.6.0, <10",
     "dominate",
+    "importlib_resources",
+    "joblib",
+    "jsonpickle",
+    "paramiko",
+    "praat-parselmouth",
     "progress",
+    "python-gettext",
     "rpdb",
+    "sphinx",
     "statsmodels",
     "tqdm",
     "yaspin",
 ]
 
-[project.urls]
-"Homepage" = "https://www.psynet.dev/"
-"Documentation" = "https://psynetdev.gitlab.io/PsyNet/"
-"Bug Tracker" = "https://gitlab.com/PsyNetDev/PsyNet/-/issues"
+[project.optional-dependencies]
+dev = [
+    "furo",
+    "isort",
+    "mock",
+    "pre-commit",
+    "sphinx-autodoc-typehints",
+]
 
 [project.scripts]
 psynet = "psynet.command_line:psynet"
 
+[project.urls]
+Changelog = "https://gitlab.com/PsyNetDev/PsyNet/-/blob/v9-master/CHANGELOG.md"
+Documentation = "https://psynetdev.gitlab.io/PsyNet/"
+Homepage = "https://www.psynet.dev/"
+Issues = "https://gitlab.com/PsyNetDev/PsyNet/-/issues"
+Repository = "https://gitlab.com/PsyNetDev/PsyNet/-/tree/v9-master"
+
 [tool.hatch.build.targets.sdist]
 exclude = [
     "/.gitlab",
     "/postgres_setup.sql",
     "/demos",
     "/docs",
     "/tests",
```

