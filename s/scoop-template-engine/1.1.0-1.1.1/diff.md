# Comparing `tmp/scoop-template-engine-1.1.0.tar.gz` & `tmp/scoop-template-engine-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoop-template-engine-1.1.0.tar", last modified: Sat Apr 29 11:17:43 2023, max compression
+gzip compressed data, was "scoop-template-engine-1.1.1.tar", last modified: Sat Apr 29 22:15:00 2023, max compression
```

## Comparing `scoop-template-engine-1.1.0.tar` & `scoop-template-engine-1.1.1.tar`

### file list

```diff
@@ -1,1213 +1,1213 @@
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.484992 scoop-template-engine-1.1.0/
--rw-------   0 roland    (1000) roland    (1000)      880 2023-04-29 10:40:17.000000 scoop-template-engine-1.1.0/CHANGELOG.md
--rw-------   0 roland    (1000) roland    (1000)     1147 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/DESCRIPTION.md
--rw-------   0 roland    (1000) roland    (1000)     1075 2023-02-11 10:49:01.000000 scoop-template-engine-1.1.0/LICENSE
--rw-------   0 roland    (1000) roland    (1000)      815 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/MANIFEST.in
--rw-------   0 roland    (1000) roland    (1000)     2421 2023-04-29 11:17:43.484992 scoop-template-engine-1.1.0/PKG-INFO
--rw-------   0 roland    (1000) roland    (1000)      818 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/README.md
--rw-------   0 roland    (1000) roland    (1000)     2635 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/pyproject.toml
--rw-------   0 roland    (1000) roland    (1000)       38 2023-04-29 11:17:43.484992 scoop-template-engine-1.1.0/setup.cfg
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.396990 scoop-template-engine-1.1.0/src/
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.400990 scoop-template-engine-1.1.0/src/doc/
--rw-------   0 roland    (1000) roland    (1000)        0 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/doc/__init__.py
--rw-------   0 roland    (1000) roland    (1000)    26799 2023-03-05 21:04:43.000000 scoop-template-engine-1.1.0/src/doc/markup.py
--rw-------   0 roland    (1000) roland    (1000)   320636 2023-04-29 11:04:55.000000 scoop-template-engine-1.1.0/src/doc/scoop-prepare-bibtex-file.pdf
--rw-------   0 roland    (1000) roland    (1000)   493112 2023-04-29 11:04:52.000000 scoop-template-engine-1.1.0/src/doc/scoop-template-engine.pdf
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.404991 scoop-template-engine-1.1.0/src/scoop_template_engine.egg-info/
--rw-------   0 roland    (1000) roland    (1000)     2421 2023-04-29 11:17:43.000000 scoop-template-engine-1.1.0/src/scoop_template_engine.egg-info/PKG-INFO
--rw-------   0 roland    (1000) roland    (1000)    62787 2023-04-29 11:17:43.000000 scoop-template-engine-1.1.0/src/scoop_template_engine.egg-info/SOURCES.txt
--rw-------   0 roland    (1000) roland    (1000)        1 2023-04-29 11:17:43.000000 scoop-template-engine-1.1.0/src/scoop_template_engine.egg-info/dependency_links.txt
--rw-------   0 roland    (1000) roland    (1000)       68 2023-04-29 11:17:43.000000 scoop-template-engine-1.1.0/src/scoop_template_engine.egg-info/entry_points.txt
--rw-------   0 roland    (1000) roland    (1000)      158 2023-04-29 11:17:43.000000 scoop-template-engine-1.1.0/src/scoop_template_engine.egg-info/requires.txt
--rw-------   0 roland    (1000) roland    (1000)       13 2023-04-29 11:17:43.000000 scoop-template-engine-1.1.0/src/scoop_template_engine.egg-info/top_level.txt
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.404991 scoop-template-engine-1.1.0/src/spbf/
--rw-------   0 roland    (1000) roland    (1000)        0 2023-02-18 12:12:19.000000 scoop-template-engine-1.1.0/src/spbf/__init__.py
--rw-------   0 roland    (1000) roland    (1000)    24233 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/spbf/__main__.py
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.404991 scoop-template-engine-1.1.0/src/ste/
--rw-------   0 roland    (1000) roland    (1000)        0 2023-02-18 12:12:19.000000 scoop-template-engine-1.1.0/src/ste/__init__.py
--rw-------   0 roland    (1000) roland    (1000)    29845 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/__main__.py
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.404991 scoop-template-engine-1.1.0/src/ste/manuscripts/
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.420991 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/
--rwx------   0 roland    (1000) roland    (1000)     1011 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/init.py
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-aabmcb.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-aaembp.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-aaemcq.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-aamick.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-aanmf6.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-aapmcd.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-aastgj.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-abmcb8.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-abseba.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-acbcct.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-accacs.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-achre4.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-achsc5.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-acncdm.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-acsccc.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-acscii.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-acsodf.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-aeacb3.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-aeacc4.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-aeecco.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-aelccp.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-aesccq.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-aewcaa.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-afsthl.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-aidcbc.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-amacgu.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-amachv.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-amclct.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-amlccd.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-amlcef.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-amrcda.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-anaccx.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-ancac3.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-ancham.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-aoiab5.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-apaccd.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-apcach.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-apchd5.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-aptsfn.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-asbcd6.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-ascecg.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-ascefj.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-bcches.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-bichaw.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-bomaf6.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-cgdefu.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-chreay.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-cmatex.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-crtoec.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-enfuem.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-esthag.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-estlcu.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-iecred.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-inocaj.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-jaaucr.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-jacsat.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-jafcau.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-jamsef.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-jceaax.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-jceda8.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-jcisd8.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-jctcce.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-jmcmar.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-jnprdf.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-joceah.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-jpcafh.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-jpcbfk.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-jpccck.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-jpclcd.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-jprobs.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-langd5.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-mamobx.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-mpohbp.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-nalefd.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-oprdfk.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-orgnd7.sty
--rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-orlef7.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-aabmcb.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-aaembp.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-aaemcq.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-aamick.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-aanmf6.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-aapmcd.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-aastgj.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-abmcb8.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-abseba.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-acbcct.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-accacs.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-achre4.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-achsc5.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-acncdm.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-acsccc.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-acscii.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-acsodf.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-aeacb3.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-aeacc4.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-aeecco.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-aelccp.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-aesccq.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-aewcaa.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-afsthl.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-aidcbc.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-amacgu.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-amachv.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-amclct.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-amlccd.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-amlcef.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-amrcda.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-anaccx.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-ancac3.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-ancham.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-aoiab5.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-apaccd.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-apcach.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-apchd5.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-aptsfn.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-asbcd6.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-ascecg.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-ascefj.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-bcches.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-bichaw.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-bomaf6.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-cgdefu.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-chreay.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-cmatex.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-crtoec.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-enfuem.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-esthag.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-estlcu.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-iecred.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-inocaj.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-jaaucr.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-jacsat.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-jafcau.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-jamsef.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-jceaax.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-jceda8.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-jcisd8.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-jctcce.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-jmcmar.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-jnprdf.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-joceah.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-jpcafh.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-jpcbfk.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-jpccck.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-jpclcd.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-jprobs.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-langd5.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-mamobx.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-mpohbp.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-nalefd.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-oprdfk.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-orgnd7.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-orlef7.sty
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-aabmcb.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-aaembp.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-aaemcq.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-aamick.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-aanmf6.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-aapmcd.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-aastgj.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-abmcb8.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-abseba.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-acbcct.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-accacs.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-achre4.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-achsc5.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-acncdm.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-acsccc.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-acscii.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-acsodf.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-aeacb3.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-aeacc4.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-aeecco.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-aelccp.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-aesccq.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-aewcaa.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-afsthl.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-aidcbc.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-amacgu.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-amachv.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-amclct.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-amlccd.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-amlcef.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-amrcda.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-anaccx.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-ancac3.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-ancham.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-aoiab5.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-apaccd.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-apcach.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-apchd5.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-aptsfn.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-asbcd6.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-ascecg.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-ascefj.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-bcches.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-bichaw.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-bomaf6.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-cgdefu.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-chreay.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-cmatex.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-crtoec.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-enfuem.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-esthag.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-estlcu.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-iecred.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-inocaj.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-jaaucr.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-jacsat.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-jafcau.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-jamsef.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-jceaax.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-jceda8.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-jcisd8.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-jctcce.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-jmcmar.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-jnprdf.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-joceah.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-jpcafh.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-jpcbfk.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-jpccck.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-jpclcd.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-jprobs.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-langd5.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-mamobx.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-mpohbp.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-nalefd.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-oprdfk.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-orgnd7.tex
--rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-orlef7.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.424991 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/
--rwx------   0 roland    (1000) roland    (1000)      655 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/init.py
--rw-------   0 roland    (1000) roland    (1000)     2561 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/postpreamble-amcomm.sty
--rw-------   0 roland    (1000) roland    (1000)     2561 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/postpreamble-cpaa.sty
--rw-------   0 roland    (1000) roland    (1000)     2561 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/postpreamble-dcds-b.sty
--rw-------   0 roland    (1000) roland    (1000)     2561 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/postpreamble-dcds-s.sty
--rw-------   0 roland    (1000) roland    (1000)     2561 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/postpreamble-dcds.sty
--rw-------   0 roland    (1000) roland    (1000)     2561 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/postpreamble-eect.sty
--rw-------   0 roland    (1000) roland    (1000)     2561 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/postpreamble-fods.sty
--rw-------   0 roland    (1000) roland    (1000)     2561 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/postpreamble-ipi.sty
--rw-------   0 roland    (1000) roland    (1000)     2561 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/postpreamble-jcd.sty
--rw-------   0 roland    (1000) roland    (1000)     2561 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/postpreamble-jdg.sty
--rw-------   0 roland    (1000) roland    (1000)     2561 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/postpreamble-jgm.sty
--rw-------   0 roland    (1000) roland    (1000)     2561 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/postpreamble-jimo.sty
--rw-------   0 roland    (1000) roland    (1000)     2561 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/postpreamble-krm.sty
--rw-------   0 roland    (1000) roland    (1000)     2561 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/postpreamble-mcrf.sty
--rw-------   0 roland    (1000) roland    (1000)     2561 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/postpreamble-mfc.sty
--rw-------   0 roland    (1000) roland    (1000)     2561 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/postpreamble-naco.sty
--rw-------   0 roland    (1000) roland    (1000)     2561 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/postpreamble-nhm.sty
--rw-------   0 roland    (1000) roland    (1000)     4187 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/template-amcomm.tex
--rw-------   0 roland    (1000) roland    (1000)     4187 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/template-cpaa.tex
--rw-------   0 roland    (1000) roland    (1000)     4187 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/template-dcds-b.tex
--rw-------   0 roland    (1000) roland    (1000)     4187 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/template-dcds-s.tex
--rw-------   0 roland    (1000) roland    (1000)     4187 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/template-dcds.tex
--rw-------   0 roland    (1000) roland    (1000)     4187 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/template-eect.tex
--rw-------   0 roland    (1000) roland    (1000)     4187 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/template-fods.tex
--rw-------   0 roland    (1000) roland    (1000)     4187 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/template-ipi.tex
--rw-------   0 roland    (1000) roland    (1000)     4187 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/template-jcd.tex
--rw-------   0 roland    (1000) roland    (1000)     4187 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/template-jdg.tex
--rw-------   0 roland    (1000) roland    (1000)     4187 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/template-jgm.tex
--rw-------   0 roland    (1000) roland    (1000)     4187 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/template-jimo.tex
--rw-------   0 roland    (1000) roland    (1000)     4187 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/template-krm.tex
--rw-------   0 roland    (1000) roland    (1000)     4187 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/template-mcrf.tex
--rw-------   0 roland    (1000) roland    (1000)     4187 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/template-mfc.tex
--rw-------   0 roland    (1000) roland    (1000)     4187 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/template-naco.tex
--rw-------   0 roland    (1000) roland    (1000)     4187 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/template-nhm.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.400990 scoop-template-engine-1.1.0/src/ste/manuscripts/AMS/
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.424991 scoop-template-engine-1.1.0/src/ste/manuscripts/AMS/mcom/
--rwx------   0 roland    (1000) roland    (1000)      984 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AMS/mcom/init.py
--rw-------   0 roland    (1000) roland    (1000)     2401 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AMS/mcom/postpreamble-mcom.sty
--rw-------   0 roland    (1000) roland    (1000)     1631 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/AMS/mcom/template-mcom.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.400990 scoop-template-engine-1.1.0/src/ste/manuscripts/Begell/
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.424991 scoop-template-engine-1.1.0/src/ste/manuscripts/Begell/ijuq/
--rw-------   0 roland    (1000) roland    (1000)      324 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Begell/ijuq/IJ4UQ_Bibliography_Style.bst.patch
--rwx------   0 roland    (1000) roland    (1000)     1326 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Begell/ijuq/init.py
--rw-------   0 roland    (1000) roland    (1000)     2888 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Begell/ijuq/postpreamble-ijuq.sty
--rw-------   0 roland    (1000) roland    (1000)     1271 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Begell/ijuq/preamble-ijuq.sty
--rw-------   0 roland    (1000) roland    (1000)     2486 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Begell/ijuq/template-ijuq.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.400990 scoop-template-engine-1.1.0/src/ste/manuscripts/Centre Mersenne/
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.424991 scoop-template-engine-1.1.0/src/ste/manuscripts/Centre Mersenne/ojmo/
--rwx------   0 roland    (1000) roland    (1000)      675 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Centre Mersenne/ojmo/init.py
--rw-------   0 roland    (1000) roland    (1000)     2763 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Centre Mersenne/ojmo/postpreamble-ojmo.sty
--rw-------   0 roland    (1000) roland    (1000)     1230 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Centre Mersenne/ojmo/preamble-ojmo.sty
--rw-------   0 roland    (1000) roland    (1000)     1966 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Centre Mersenne/ojmo/template-ojmo.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.400990 scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.424991 scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/acvar/
--rw-------   0 roland    (1000) roland    (1000)      699 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/acvar/init.py
--rw-------   0 roland    (1000) roland    (1000)     2153 2023-04-29 10:06:57.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/acvar/postpreamble-acvar.sty
--rw-------   0 roland    (1000) roland    (1000)     2525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/acvar/template-acvar.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.424991 scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/cmam/
--rwx------   0 roland    (1000) roland    (1000)      711 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/cmam/init.py
--rw-------   0 roland    (1000) roland    (1000)     2153 2023-04-29 10:06:57.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/cmam/postpreamble-cmam.sty
--rw-------   0 roland    (1000) roland    (1000)     2525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/cmam/template-cmam.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.424991 scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/crelle/
--rwx------   0 roland    (1000) roland    (1000)     1240 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/crelle/init.py
--rw-------   0 roland    (1000) roland    (1000)     2574 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/crelle/postpreamble-crelle.sty
--rw-------   0 roland    (1000) roland    (1000)     1262 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/crelle/preamble-crelle.sty
--rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/crelle/prepreamble-crelle.sty
--rw-------   0 roland    (1000) roland    (1000)     1771 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/crelle/template-crelle.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.424991 scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/jip/
--rwx------   0 roland    (1000) roland    (1000)      707 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/jip/init.py
--rw-------   0 roland    (1000) roland    (1000)     2153 2023-04-29 10:06:57.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/jip/postpreamble-jip.sty
--rw-------   0 roland    (1000) roland    (1000)     2525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/jip/template-jip.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.424991 scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/jnm/
--rwx------   0 roland    (1000) roland    (1000)      698 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/jnm/init.py
--rw-------   0 roland    (1000) roland    (1000)     2153 2023-04-29 10:06:57.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/jnm/postpreamble-jnm.sty
--rw-------   0 roland    (1000) roland    (1000)     2525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/jnm/template-jnm.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.400990 scoop-template-engine-1.1.0/src/ste/manuscripts/EMS/
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.424991 scoop-template-engine-1.1.0/src/ste/manuscripts/EMS/ag/
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/EMS/ag/postpreamble-ag.sty
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/EMS/ag/template-ag.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.424991 scoop-template-engine-1.1.0/src/ste/manuscripts/EMS/em/
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/EMS/em/postpreamble-em.sty
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/EMS/em/template-em.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.424991 scoop-template-engine-1.1.0/src/ste/manuscripts/EMS/rlm/
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/EMS/rlm/postpreamble-rlm.sty
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/EMS/rlm/template-rlm.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.400990 scoop-template-engine-1.1.0/src/ste/manuscripts/ESAIM/
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.424991 scoop-template-engine-1.1.0/src/ste/manuscripts/ESAIM/cocv/
--rwx------   0 roland    (1000) roland    (1000)     1123 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ESAIM/cocv/init.py
--rw-------   0 roland    (1000) roland    (1000)     2340 2023-04-29 10:01:35.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ESAIM/cocv/postpreamble-cocv.sty
--rw-------   0 roland    (1000) roland    (1000)     1714 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ESAIM/cocv/template-cocv.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.428991 scoop-template-engine-1.1.0/src/ste/manuscripts/ESAIM/m2an/
--rwx------   0 roland    (1000) roland    (1000)     1120 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ESAIM/m2an/init.py
--rw-------   0 roland    (1000) roland    (1000)     2340 2023-04-29 10:01:30.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ESAIM/m2an/postpreamble-m2an.sty
--rw-------   0 roland    (1000) roland    (1000)     1708 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/ESAIM/m2an/template-m2an.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.400990 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.452991 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/
--rwx------   0 roland    (1000) roland    (1000)     1604 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/init.py
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-aam.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-acha.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-advengsoft.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-aim.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-amc.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-aml.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-apal.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-apm.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-apnum.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-arcontrol.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-array.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-bcra.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-bdr.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-bica.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-brain.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-bulsci.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-cad.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-cam.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-camwa.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-chaos.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-cma.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-cnsns.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-cocom.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-coisb.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-cola.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-comgeo.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-commatsci.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-compgeo.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-compstruc.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-conengprac.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-cosrev.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-cpc.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-csda.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-csfx.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-csl.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-dajour.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-dam.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-dark.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-difgeo.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-disc.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-disopt.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ecocom.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ecolmodel.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ecosta.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ejc.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ejor.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-enganabound.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-engappai.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-exco.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-exmath.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ffa.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-finel.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-fss.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-geb.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-geomphys.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-gmod.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-hcc.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-health.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-heliyon.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ic.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ijforecast.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ime.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-indag.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ins.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ipl.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jaca.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jalgebra.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jat.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jcmds.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jco.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jcp.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jcpx.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jcss.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jcta.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jctb.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jde.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jebo.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jeconom.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jedc.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jet.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jfa.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jfranklin.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jlamp.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jmaa.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jmateco.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jnt.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jocsci.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jpaa.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jprocont.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jspi.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jsymbc.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-laa.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-matcom.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-matpur.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-mbs.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-mlwa.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-mss.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-na.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-nahs.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-nanocomnet.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-neunet.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-nlm.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-nonrwa.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-nppp.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-nuclphysb.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-orl.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-padiff.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-patterns.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-physa.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-physd.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-physleta.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-physletb.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-plrev.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-pmc.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-pr.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-red.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-rico.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-rinam.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-sasc.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-spa.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-spasta.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-stapro.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-swevo.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-sysconle.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-tcs.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-topol.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-vehcom.sty
--rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-wace.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-aam.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-acha.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-advengsoft.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-aim.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-amc.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-aml.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-apal.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-apm.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-apnum.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-arcontrol.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-array.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-bcra.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-bdr.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-bica.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-brain.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-bulsci.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-cad.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-cam.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-camwa.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-chaos.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-cma.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-cnsns.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-cocom.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-coisb.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-cola.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-comgeo.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-commatsci.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-compgeo.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-compstruc.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-conengprac.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-cosrev.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-cpc.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-csda.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-csfx.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-csl.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-dajour.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-dam.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-dark.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-difgeo.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-disc.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-disopt.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ecocom.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ecolmodel.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ecosta.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ejc.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ejor.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-enganabound.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-engappai.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-exco.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-exmath.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ffa.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-finel.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-fss.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-geb.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-geomphys.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-gmod.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-hcc.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-health.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-heliyon.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ic.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ijforecast.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ime.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-indag.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ins.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ipl.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jaca.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jalgebra.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jat.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jcmds.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jco.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jcp.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jcpx.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jcss.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jcta.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jctb.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jde.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jebo.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jeconom.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jedc.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jet.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jfa.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jfranklin.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jlamp.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jmaa.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jmateco.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jnt.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jocsci.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jpaa.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jprocont.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jspi.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jsymbc.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-laa.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-matcom.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-matpur.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-mbs.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-mlwa.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-mss.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-na.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-nahs.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-nanocomnet.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-neunet.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-nlm.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-nonrwa.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-nppp.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-nuclphysb.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-orl.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-padiff.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-patterns.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-physa.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-physd.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-physleta.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-physletb.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-plrev.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-pmc.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-pr.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-red.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-rico.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-rinam.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-sasc.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-spa.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-spasta.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-stapro.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-swevo.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-sysconle.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-tcs.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-topol.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-vehcom.sty
--rw-------   0 roland    (1000) roland    (1000)     1118 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-wace.sty
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-aam.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-acha.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-advengsoft.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-aim.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-amc.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-aml.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-apal.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-apm.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-apnum.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-arcontrol.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-array.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-bcra.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-bdr.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-bica.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-brain.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-bulsci.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-cad.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-cam.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-camwa.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-chaos.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-cma.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-cnsns.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-cocom.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-coisb.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-cola.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-comgeo.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-commatsci.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-compgeo.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-compstruc.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-conengprac.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-cosrev.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-cpc.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-csda.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-csfx.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-csl.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-dajour.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-dam.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-dark.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-difgeo.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-disc.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-disopt.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ecocom.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ecolmodel.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ecosta.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ejc.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ejor.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-enganabound.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-engappai.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-exco.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-exmath.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ffa.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-finel.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-fss.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-geb.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-geomphys.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-gmod.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-hcc.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-health.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-heliyon.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ic.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ijforecast.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ime.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-indag.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ins.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ipl.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jaca.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jalgebra.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jat.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jcmds.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jco.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jcp.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jcpx.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jcss.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jcta.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jctb.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jde.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jebo.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jeconom.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jedc.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jet.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jfa.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jfranklin.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jlamp.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jmaa.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jmateco.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jnt.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jocsci.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jpaa.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jprocont.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jspi.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jsymbc.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-laa.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-matcom.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-matpur.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-mbs.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-mlwa.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-mss.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-na.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-nahs.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-nanocomnet.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-neunet.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-nlm.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-nonrwa.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-nppp.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-nuclphysb.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-orl.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-padiff.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-patterns.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-physa.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-physd.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-physleta.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-physletb.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-plrev.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-pmc.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-pr.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-red.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-rico.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-rinam.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-sasc.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-spa.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-spasta.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-stapro.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-swevo.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-sysconle.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-tcs.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-topol.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-vehcom.tex
--rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-wace.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.452991 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/ifac/
--rwx------   0 roland    (1000) roland    (1000)      788 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/ifac/init.py
--rw-------   0 roland    (1000) roland    (1000)     2998 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/ifac/postpreamble-ifac.sty
--rw-------   0 roland    (1000) roland    (1000)     1307 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/ifac/preamble-ifac.sty
--rw-------   0 roland    (1000) roland    (1000)     1851 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/ifac/template-ifac.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.452991 scoop-template-engine-1.1.0/src/ste/manuscripts/Frontiers/
--rwx------   0 roland    (1000) roland    (1000)      706 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Frontiers/init.py
--rw-------   0 roland    (1000) roland    (1000)     2812 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Frontiers/postpreamble-fams.sty
--rw-------   0 roland    (1000) roland    (1000)     2404 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Frontiers/template-fams.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.464991 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/
--rw-------   0 roland    (1000) roland    (1000)     1093 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/init.py
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-bbiici.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-bioffn.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-bmbucs.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-bpeeae.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-cqgrdg.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-dmatb7.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-ejphd4.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-ejssbg.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-erc.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-ercl.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-ere.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-erenbl.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-erh.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-erisal.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-erlnal.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-esltac.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-fcsuah.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-fpelab.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-ijemkf.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-ip.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-isoccm.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-jbrobw.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-jcapbp.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-jcomel.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-jionas.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-jmmiez.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-jneiez.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-joopca.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-jpamb5.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-jpapbe.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-jpapeh.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-jpcofp.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-jpcogq.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-jpeoey.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-jpgped.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-jpmoc4.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-jppokr.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-jrprea.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-jsmtc6.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-mafeb2.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-mlstck.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-mmuabd.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-mqtaaz.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-mreac3.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-msmeeu.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-mstcep.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-mtrgau.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-nceecn.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-neaxa4.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-nfaub3.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-njopfm.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-nnoter.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-nonle5.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-nufuau.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-pberb8.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-pbhiat.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-perndg.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-pheda7.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-phmba7.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-phstbo.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-pmeae3.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-ppcfet.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-prelcz.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-psteeu.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-qstuah.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-rpphag.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-smster.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-ssteet.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-stmpcw.sty
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-sustef.sty
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-bbiici.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-bioffn.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-bmbucs.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-bpeeae.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-cqgrdg.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-dmatb7.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-ejphd4.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-ejssbg.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-erc.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-ercl.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-ere.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-erenbl.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-erh.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-erisal.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-erlnal.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-esltac.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-fcsuah.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-fpelab.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-ijemkf.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-ip.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-isoccm.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-jbrobw.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-jcapbp.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-jcomel.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-jionas.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-jmmiez.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-jneiez.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-joopca.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-jpamb5.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-jpapbe.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-jpapeh.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-jpcofp.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-jpcogq.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-jpeoey.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-jpgped.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-jpmoc4.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-jppokr.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-jrprea.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-jsmtc6.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-mafeb2.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-mlstck.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-mmuabd.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-mqtaaz.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-mreac3.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-msmeeu.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-mstcep.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-mtrgau.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-nceecn.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-neaxa4.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-nfaub3.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-njopfm.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-nnoter.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-nonle5.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-nufuau.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-pberb8.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-pbhiat.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-perndg.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-pheda7.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-phmba7.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-phstbo.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-pmeae3.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-ppcfet.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-prelcz.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-psteeu.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-qstuah.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-rpphag.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-smster.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-ssteet.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-stmpcw.tex
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-sustef.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.400990 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.468992 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/
--r--------   0 roland    (1000) roland    (1000)     2449 2023-04-29 11:14:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-aa.sty
--r--------   0 roland    (1000) roland    (1000)     2599 2023-04-29 11:14:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-acdm.sty
--r--------   0 roland    (1000) roland    (1000)     2247 2023-04-29 11:14:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-amspreprint.sty
--r--------   0 roland    (1000) roland    (1000)     2773 2023-04-29 11:14:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-bit.sty
--r--------   0 roland    (1000) roland    (1000)     2275 2023-04-29 11:14:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-cma.sty
--r--------   0 roland    (1000) roland    (1000)     2153 2023-04-29 11:14:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-cmam.sty
--r--------   0 roland    (1000) roland    (1000)     2340 2023-04-29 11:14:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-cocv.sty
--r--------   0 roland    (1000) roland    (1000)     2574 2023-04-29 11:14:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-crelle.sty
--r--------   0 roland    (1000) roland    (1000)     3123 2023-04-29 11:14:28.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-etna.sty
--r--------   0 roland    (1000) roland    (1000)     2812 2023-04-29 11:14:28.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-fams.sty
--r--------   0 roland    (1000) roland    (1000)     2417 2023-04-29 11:14:32.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-gamm.sty
--r--------   0 roland    (1000) roland    (1000)     2419 2023-04-29 11:14:32.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-iecred.sty
--r--------   0 roland    (1000) roland    (1000)     2998 2023-04-29 11:14:32.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-ifac.sty
--r--------   0 roland    (1000) roland    (1000)     2490 2023-04-29 11:14:32.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-ijcga.sty
--r--------   0 roland    (1000) roland    (1000)     3231 2023-04-29 11:14:32.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-ijcm.sty
--r--------   0 roland    (1000) roland    (1000)     2888 2023-04-29 11:14:32.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-ijuq.sty
--r--------   0 roland    (1000) roland    (1000)     2302 2023-04-29 11:14:32.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-imanum.sty
--r--------   0 roland    (1000) roland    (1000)     2277 2023-04-29 11:14:33.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-jmiv.sty
--r--------   0 roland    (1000) roland    (1000)     1976 2023-04-29 11:14:37.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-jnsao.sty
--r--------   0 roland    (1000) roland    (1000)     2774 2023-04-29 11:14:37.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-jota.sty
--r--------   0 roland    (1000) roland    (1000)     2773 2023-04-29 11:14:37.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-jsc.sty
--r--------   0 roland    (1000) roland    (1000)     2340 2023-04-29 11:14:37.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-m2an.sty
--r--------   0 roland    (1000) roland    (1000)     2498 2023-04-29 11:14:37.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-m3as.sty
--r--------   0 roland    (1000) roland    (1000)     2401 2023-04-29 11:14:37.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-mcom.sty
--r--------   0 roland    (1000) roland    (1000)     2561 2023-04-29 11:14:38.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-mcrf.sty
--r--------   0 roland    (1000) roland    (1000)     2050 2023-04-29 11:14:38.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-mma.sty
--r--------   0 roland    (1000) roland    (1000)     2050 2023-04-29 11:14:42.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-nla.sty
--r--------   0 roland    (1000) roland    (1000)     2050 2023-04-29 11:14:42.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-nme.sty
--r--------   0 roland    (1000) roland    (1000)     2763 2023-04-29 11:14:42.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-ojmo.sty
--r--------   0 roland    (1000) roland    (1000)     2582 2023-04-29 11:14:42.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-opt.sty
--r--------   0 roland    (1000) roland    (1000)     3007 2023-04-29 11:14:42.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-pamm.sty
--r--------   0 roland    (1000) roland    (1000)     2497 2023-04-29 11:14:43.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-ppl.sty
--r--------   0 roland    (1000) roland    (1000)     2219 2023-04-29 11:14:43.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-siims.sty
--r--------   0 roland    (1000) roland    (1000)     2219 2023-04-29 11:14:43.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-siopt.sty
--r--------   0 roland    (1000) roland    (1000)     2417 2023-04-29 11:14:47.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-zamm.sty
--r--------   0 roland    (1000) roland    (1000)     1345 2023-04-29 11:14:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/preamble-acdm.sty
--r--------   0 roland    (1000) roland    (1000)     1113 2023-04-29 11:14:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/preamble-bit.sty
--r--------   0 roland    (1000) roland    (1000)     1262 2023-04-29 11:14:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/preamble-crelle.sty
--r--------   0 roland    (1000) roland    (1000)     1307 2023-04-29 11:14:32.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/preamble-ifac.sty
--r--------   0 roland    (1000) roland    (1000)     1340 2023-04-29 11:14:32.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/preamble-ijcm.sty
--r--------   0 roland    (1000) roland    (1000)     1271 2023-04-29 11:14:32.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/preamble-ijuq.sty
--r--------   0 roland    (1000) roland    (1000)     1115 2023-04-29 11:14:33.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/preamble-jmiv.sty
--r--------   0 roland    (1000) roland    (1000)     1114 2023-04-29 11:14:37.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/preamble-jota.sty
--r--------   0 roland    (1000) roland    (1000)     1113 2023-04-29 11:14:37.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/preamble-jsc.sty
--r--------   0 roland    (1000) roland    (1000)     1230 2023-04-29 11:14:42.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/preamble-ojmo.sty
--r--------   0 roland    (1000) roland    (1000)     1118 2023-04-29 11:14:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/prepreamble-cma.sty
--r--------   0 roland    (1000) roland    (1000)     1194 2023-04-29 11:14:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/prepreamble-crelle.sty
--r--------   0 roland    (1000) roland    (1000)     1116 2023-04-29 11:14:28.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/prepreamble-etna.sty
--r--------   0 roland    (1000) roland    (1000)     1194 2023-04-29 11:14:32.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/prepreamble-iecred.sty
--r--------   0 roland    (1000) roland    (1000)     1304 2023-04-29 11:14:32.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/prepreamble-imanum.sty
--r--------   0 roland    (1000) roland    (1000)     1525 2023-04-29 11:14:33.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/prepreamble-jmiv.sty
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.400990 scoop-template-engine-1.1.0/src/ste/manuscripts/Oxford Academic/
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.468992 scoop-template-engine-1.1.0/src/ste/manuscripts/Oxford Academic/imanum/
--rwx------   0 roland    (1000) roland    (1000)      923 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Oxford Academic/imanum/init.py
--rw-------   0 roland    (1000) roland    (1000)     2302 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Oxford Academic/imanum/postpreamble-imanum.sty
--rw-------   0 roland    (1000) roland    (1000)     1304 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Oxford Academic/imanum/prepreamble-imanum.sty
--rw-------   0 roland    (1000) roland    (1000)     2325 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Oxford Academic/imanum/template-imanum.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.472992 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/
--rwx------   0 roland    (1000) roland    (1000)      812 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/init.py
--rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/postpreamble-mms.sty
--rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/postpreamble-siap.sty
--rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/postpreamble-sicomp.sty
--rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/postpreamble-sicon.sty
--rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/postpreamble-sidma.sty
--rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/postpreamble-sima.sty
--rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/postpreamble-simax.sty
--rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/postpreamble-sinum.sty
--rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/postpreamble-siopt.sty
--rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/postpreamble-sirev.sty
--rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/postpreamble-sisc.sty
--rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/postpreamble-tvp.sty
--rw-------   0 roland    (1000) roland    (1000)     3236 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/template-mms.tex
--rw-------   0 roland    (1000) roland    (1000)     3236 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/template-siap.tex
--rw-------   0 roland    (1000) roland    (1000)     3236 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/template-sicomp.tex
--rw-------   0 roland    (1000) roland    (1000)     3236 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/template-sicon.tex
--rw-------   0 roland    (1000) roland    (1000)     3236 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/template-sidma.tex
--rw-------   0 roland    (1000) roland    (1000)     3236 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/template-sima.tex
--rw-------   0 roland    (1000) roland    (1000)     3236 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/template-simax.tex
--rw-------   0 roland    (1000) roland    (1000)     3236 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/template-sinum.tex
--rw-------   0 roland    (1000) roland    (1000)     3236 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/template-siopt.tex
--rw-------   0 roland    (1000) roland    (1000)     3236 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/template-sirev.tex
--rw-------   0 roland    (1000) roland    (1000)     3236 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/template-sisc.tex
--rw-------   0 roland    (1000) roland    (1000)     3236 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/template-tvp.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.472992 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAMOnline/
--rwx------   0 roland    (1000) roland    (1000)      814 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAMOnline/init.py
--rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAMOnline/postpreamble-juq.sty
--rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAMOnline/postpreamble-siads.sty
--rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAMOnline/postpreamble-siaga.sty
--rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAMOnline/postpreamble-sifin.sty
--rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAMOnline/postpreamble-siims.sty
--rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAMOnline/postpreamble-simods.sty
--rw-------   0 roland    (1000) roland    (1000)     2595 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAMOnline/template-juq.tex
--rw-------   0 roland    (1000) roland    (1000)     2595 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAMOnline/template-siads.tex
--rw-------   0 roland    (1000) roland    (1000)     2595 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAMOnline/template-siaga.tex
--rw-------   0 roland    (1000) roland    (1000)     2595 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAMOnline/template-sifin.tex
--rw-------   0 roland    (1000) roland    (1000)     2595 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAMOnline/template-siims.tex
--rw-------   0 roland    (1000) roland    (1000)     2595 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/SIAMOnline/template-simods.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.400990 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.472992 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bit/
--rw-------   0 roland    (1000) roland    (1000)     1321 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bit/init.py
--rw-------   0 roland    (1000) roland    (1000)     2773 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bit/postpreamble-bit.sty
--rw-------   0 roland    (1000) roland    (1000)     1113 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bit/preamble-bit.sty
--rw-------   0 roland    (1000) roland    (1000)     2221 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bit/template-bit.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.472992 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bmcart.cls/
--rw-------   0 roland    (1000) roland    (1000)      864 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bmcart.cls/init.py
--rw-------   0 roland    (1000) roland    (1000)     2599 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bmcart.cls/postpreamble-acdm.sty
--rw-------   0 roland    (1000) roland    (1000)     2599 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bmcart.cls/postpreamble-bvp.sty
--rw-------   0 roland    (1000) roland    (1000)     2599 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bmcart.cls/postpreamble-jia.sty
--rw-------   0 roland    (1000) roland    (1000)     2599 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bmcart.cls/postpreamble-jmi.sty
--rw-------   0 roland    (1000) roland    (1000)     1345 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bmcart.cls/preamble-acdm.sty
--rw-------   0 roland    (1000) roland    (1000)     1345 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bmcart.cls/preamble-bvp.sty
--rw-------   0 roland    (1000) roland    (1000)     1345 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bmcart.cls/preamble-jia.sty
--rw-------   0 roland    (1000) roland    (1000)     1345 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bmcart.cls/preamble-jmi.sty
--rw-------   0 roland    (1000) roland    (1000)     2353 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bmcart.cls/template-acdm.tex
--rw-------   0 roland    (1000) roland    (1000)     2353 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bmcart.cls/template-bvp.tex
--rw-------   0 roland    (1000) roland    (1000)     2353 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bmcart.cls/template-jia.tex
--rw-------   0 roland    (1000) roland    (1000)     2353 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bmcart.cls/template-jmi.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.472992 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/jota/
--rw-------   0 roland    (1000) roland    (1000)      955 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/jota/init.py
--rw-------   0 roland    (1000) roland    (1000)     2774 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/jota/postpreamble-jota.sty
--rw-------   0 roland    (1000) roland    (1000)     1114 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/jota/preamble-jota.sty
--rw-------   0 roland    (1000) roland    (1000)     2148 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/jota/template-jota.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.480992 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/
--rw-------   0 roland    (1000) roland    (1000)      847 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/init.py
--rw-------   0 roland    (1000) roland    (1000)     2277 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-acom.sty
--rw-------   0 roland    (1000) roland    (1000)     2277 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-amo.sty
--rw-------   0 roland    (1000) roland    (1000)     2277 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-calcolo.sty
--rw-------   0 roland    (1000) roland    (1000)     2277 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-camcos.sty
--rw-------   0 roland    (1000) roland    (1000)     2277 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-cm.sty
--rw-------   0 roland    (1000) roland    (1000)     2277 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-coam.sty
--rw-------   0 roland    (1000) roland    (1000)     2277 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-coap.sty
--rw-------   0 roland    (1000) roland    (1000)     2277 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-cvpde.sty
--rw-------   0 roland    (1000) roland    (1000)     2277 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-dcg.sty
--rw-------   0 roland    (1000) roland    (1000)     2277 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-focm.sty
--rw-------   0 roland    (1000) roland    (1000)     2277 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-ijot.sty
--rw-------   0 roland    (1000) roland    (1000)     2277 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-inge.sty
--rw-------   0 roland    (1000) roland    (1000)     2277 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-jmiv.sty
--rw-------   0 roland    (1000) roland    (1000)     2277 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-jogo.sty
--rw-------   0 roland    (1000) roland    (1000)     2277 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-maana.sty
--rw-------   0 roland    (1000) roland    (1000)     2277 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-mathbio.sty
--rw-------   0 roland    (1000) roland    (1000)     2277 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-mathprog.sty
--rw-------   0 roland    (1000) roland    (1000)     2277 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-mmor.sty
--rw-------   0 roland    (1000) roland    (1000)     2277 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-ms.sty
--rw-------   0 roland    (1000) roland    (1000)     2277 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-numa.sty
--rw-------   0 roland    (1000) roland    (1000)     2277 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-numalg.sty
--rw-------   0 roland    (1000) roland    (1000)     2277 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-pdea.sty
--rw-------   0 roland    (1000) roland    (1000)     2277 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-rm.sty
--rw-------   0 roland    (1000) roland    (1000)     2277 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-svva.sty
--rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-acom.sty
--rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-amo.sty
--rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-calcolo.sty
--rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-camcos.sty
--rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-cm.sty
--rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-coam.sty
--rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-coap.sty
--rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-cvpde.sty
--rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-dcg.sty
--rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-focm.sty
--rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-ijot.sty
--rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-inge.sty
--rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-jmiv.sty
--rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-jogo.sty
--rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-maana.sty
--rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-mathbio.sty
--rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-mathprog.sty
--rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-mmor.sty
--rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-ms.sty
--rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-numa.sty
--rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-numalg.sty
--rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-pdea.sty
--rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-rm.sty
--rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-svva.sty
--rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-acom.sty
--rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-amo.sty
--rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-calcolo.sty
--rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-camcos.sty
--rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-cm.sty
--rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-coam.sty
--rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-coap.sty
--rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-cvpde.sty
--rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-dcg.sty
--rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-focm.sty
--rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-ijot.sty
--rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-inge.sty
--rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-jmiv.sty
--rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-jogo.sty
--rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-maana.sty
--rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-mathbio.sty
--rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-mathprog.sty
--rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-mmor.sty
--rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-ms.sty
--rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-numa.sty
--rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-numalg.sty
--rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-pdea.sty
--rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-rm.sty
--rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-svva.sty
--rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-acom.tex
--rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-amo.tex
--rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-calcolo.tex
--rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-camcos.tex
--rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-cm.tex
--rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-coam.tex
--rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-coap.tex
--rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-cvpde.tex
--rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-dcg.tex
--rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-focm.tex
--rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-ijot.tex
--rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-inge.tex
--rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-jmiv.tex
--rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-jogo.tex
--rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-maana.tex
--rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-mathbio.tex
--rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-mathprog.tex
--rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-mmor.tex
--rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-ms.tex
--rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-numa.tex
--rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-numalg.tex
--rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-pdea.tex
--rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-rm.tex
--rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-svva.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.480992 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/svjour3.cls/
--rw-------   0 roland    (1000) roland    (1000)      744 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/svjour3.cls/init.py
--rw-------   0 roland    (1000) roland    (1000)     2773 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/svjour3.cls/postpreamble-jsc.sty
--rw-------   0 roland    (1000) roland    (1000)     2773 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/svjour3.cls/postpreamble-mpc.sty
--rw-------   0 roland    (1000) roland    (1000)     2773 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/svjour3.cls/postpreamble-opte.sty
--rw-------   0 roland    (1000) roland    (1000)     1113 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/svjour3.cls/preamble-jsc.sty
--rw-------   0 roland    (1000) roland    (1000)     1113 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/svjour3.cls/preamble-mpc.sty
--rw-------   0 roland    (1000) roland    (1000)     1113 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/svjour3.cls/preamble-opte.sty
--rw-------   0 roland    (1000) roland    (1000)     2436 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/svjour3.cls/template-jsc.tex
--rw-------   0 roland    (1000) roland    (1000)     2436 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/svjour3.cls/template-mpc.tex
--rw-------   0 roland    (1000) roland    (1000)     2436 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/svjour3.cls/template-opte.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.480992 scoop-template-engine-1.1.0/src/ste/manuscripts/TaylorAndFrancis/
--rwx------   0 roland    (1000) roland    (1000)      806 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/TaylorAndFrancis/init.py
--rw-------   0 roland    (1000) roland    (1000)     2582 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/TaylorAndFrancis/postpreamble-apa.sty
--rw-------   0 roland    (1000) roland    (1000)     2582 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/TaylorAndFrancis/postpreamble-eno.sty
--rw-------   0 roland    (1000) roland    (1000)     2582 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/TaylorAndFrancis/postpreamble-oms.sty
--rw-------   0 roland    (1000) roland    (1000)     2582 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/TaylorAndFrancis/postpreamble-opt.sty
--rw-------   0 roland    (1000) roland    (1000)     2353 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/TaylorAndFrancis/template-apa.tex
--rw-------   0 roland    (1000) roland    (1000)     2353 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/TaylorAndFrancis/template-eno.tex
--rw-------   0 roland    (1000) roland    (1000)     2353 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/TaylorAndFrancis/template-oms.tex
--rw-------   0 roland    (1000) roland    (1000)     2353 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/TaylorAndFrancis/template-opt.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.400990 scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.480992 scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/gamm/
--rwx------   0 roland    (1000) roland    (1000)     1596 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/gamm/init.py
--rw-------   0 roland    (1000) roland    (1000)     2417 2023-04-29 10:00:32.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/gamm/postpreamble-gamm.sty
--rw-------   0 roland    (1000) roland    (1000)     2041 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/gamm/template-gamm.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.480992 scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/mma/
--rwx------   0 roland    (1000) roland    (1000)     2197 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/mma/init.py
--rw-------   0 roland    (1000) roland    (1000)     2050 2023-04-29 10:00:42.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/mma/postpreamble-mma.sty
--rw-------   0 roland    (1000) roland    (1000)     2405 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/mma/template-mma.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.480992 scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/nla/
--rwx------   0 roland    (1000) roland    (1000)     2125 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/nla/init.py
--rw-------   0 roland    (1000) roland    (1000)     2050 2023-04-29 10:00:54.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/nla/postpreamble-nla.sty
--rw-------   0 roland    (1000) roland    (1000)     2011 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/nla/template-nla.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.480992 scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/nme/
--rwx------   0 roland    (1000) roland    (1000)     2207 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/nme/init.py
--rw-------   0 roland    (1000) roland    (1000)     2050 2023-04-29 10:00:37.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/nme/postpreamble-nme.sty
--rw-------   0 roland    (1000) roland    (1000)     2433 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/nme/template-nme.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.480992 scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/pamm/
--rwx------   0 roland    (1000) roland    (1000)      732 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/pamm/init.py
--rw-------   0 roland    (1000) roland    (1000)     3007 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/pamm/postpreamble-pamm.sty
--rw-------   0 roland    (1000) roland    (1000)     1871 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/pamm/template-pamm.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.480992 scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/zamm/
--rwx------   0 roland    (1000) roland    (1000)     1640 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/zamm/init.py
--rw-------   0 roland    (1000) roland    (1000)     2417 2023-04-29 10:00:28.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/zamm/postpreamble-zamm.sty
--rw-------   0 roland    (1000) roland    (1000)     2019 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/zamm/template-zamm.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.400990 scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.480992 scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/aa/
--rwx------   0 roland    (1000) roland    (1000)      930 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/aa/init.py
--rw-------   0 roland    (1000) roland    (1000)     2449 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/aa/postpreamble-aa.sty
--rw-------   0 roland    (1000) roland    (1000)     1980 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/aa/template-aa.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.480992 scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/ijcga/
--rwx------   0 roland    (1000) roland    (1000)      831 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/ijcga/init.py
--rw-------   0 roland    (1000) roland    (1000)     2490 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/ijcga/postpreamble-ijcga.sty
--rw-------   0 roland    (1000) roland    (1000)     1966 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/ijcga/template-ijcga.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.480992 scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/ijcm/
--rwx------   0 roland    (1000) roland    (1000)      810 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/ijcm/init.py
--rw-------   0 roland    (1000) roland    (1000)     3231 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/ijcm/postpreamble-ijcm.sty
--rw-------   0 roland    (1000) roland    (1000)     1340 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/ijcm/preamble-ijcm.sty
--rw-------   0 roland    (1000) roland    (1000)     2023 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/ijcm/template-ijcm.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.484992 scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/m3as/
--rwx------   0 roland    (1000) roland    (1000)      815 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/m3as/init.py
--rw-------   0 roland    (1000) roland    (1000)     2498 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/m3as/postpreamble-m3as.sty
--rw-------   0 roland    (1000) roland    (1000)     2065 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/m3as/template-m3as.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.484992 scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/ppl/
--rwx------   0 roland    (1000) roland    (1000)     1221 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/ppl/init.py
--rw-------   0 roland    (1000) roland    (1000)     2497 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/ppl/postpreamble-ppl.sty
--rw-------   0 roland    (1000) roland    (1000)     2155 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/ppl/template-ppl.tex
--rw-------   0 roland    (1000) roland    (1000)     1340 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/ppl/ws-ppl.bst.patch
--rw-------   0 roland    (1000) roland    (1000)        0 2023-02-18 12:12:19.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/__init__.py
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.484992 scoop-template-engine-1.1.0/src/ste/manuscripts/etna/
--rw-------   0 roland    (1000) roland    (1000)     2773 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/etna/etna.cls.patch
--rwx------   0 roland    (1000) roland    (1000)     1685 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/etna/init.py
--rw-------   0 roland    (1000) roland    (1000)     3123 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/etna/postpreamble-etna.sty
--rw-------   0 roland    (1000) roland    (1000)     1116 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/etna/prepreamble-etna.sty
--rw-------   0 roland    (1000) roland    (1000)     2111 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/etna/template-etna.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.484992 scoop-template-engine-1.1.0/src/ste/manuscripts/jnsao/
--rwx------   0 roland    (1000) roland    (1000)      661 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/jnsao/init.py
--rw-------   0 roland    (1000) roland    (1000)     1976 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/jnsao/postpreamble-jnsao.sty
--rw-------   0 roland    (1000) roland    (1000)     1678 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/jnsao/template-jnsao.tex
--rw-------   0 roland    (1000) roland    (1000)   107629 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/manuscripts.py
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.484992 scoop-template-engine-1.1.0/src/ste/manuscripts/scoop/
--rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/scoop/postpreamble-amspreprint.sty
--rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/scoop/template-amspreprint.tex
--rw-------   0 roland    (1000) roland    (1000)      520 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/manuscripts/scoop/template-bibgenerator.tex
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.400990 scoop-template-engine-1.1.0/src/ste/schemes/
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.484992 scoop-template-engine-1.1.0/src/ste/schemes/manuscript/
--rw-------   0 roland    (1000) roland    (1000)      132 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/schemes/manuscript/abstract.tex
--rw-------   0 roland    (1000) roland    (1000)      213 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/schemes/manuscript/content.tex
--rw-------   0 roland    (1000) roland    (1000)      388 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/schemes/manuscript/manuscript.bib
--rw-------   0 roland    (1000) roland    (1000)       73 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/schemes/manuscript/manuscript.sty
--rw-------   0 roland    (1000) roland    (1000)     1433 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.0/src/ste/schemes/manuscript/manuscript.yaml
-drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 11:17:43.484992 scoop-template-engine-1.1.0/src/ste/utilities/
--rw-------   0 roland    (1000) roland    (1000)        0 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/utilities/__init__.py
--rw-------   0 roland    (1000) roland    (1000)     9510 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.0/src/ste/utilities/utilities.py
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.443385 scoop-template-engine-1.1.1/
+-rw-------   0 roland    (1000) roland    (1000)      926 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/CHANGELOG.md
+-rw-------   0 roland    (1000) roland    (1000)     1147 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/DESCRIPTION.md
+-rw-------   0 roland    (1000) roland    (1000)     1075 2023-02-11 10:49:01.000000 scoop-template-engine-1.1.1/LICENSE
+-rw-------   0 roland    (1000) roland    (1000)      815 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/MANIFEST.in
+-rw-------   0 roland    (1000) roland    (1000)     2421 2023-04-29 22:15:00.443385 scoop-template-engine-1.1.1/PKG-INFO
+-rw-------   0 roland    (1000) roland    (1000)      818 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/README.md
+-rw-------   0 roland    (1000) roland    (1000)     2635 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/pyproject.toml
+-rw-------   0 roland    (1000) roland    (1000)       38 2023-04-29 22:15:00.443385 scoop-template-engine-1.1.1/setup.cfg
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.371385 scoop-template-engine-1.1.1/src/
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.375385 scoop-template-engine-1.1.1/src/doc/
+-rw-------   0 roland    (1000) roland    (1000)        0 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/doc/__init__.py
+-rw-------   0 roland    (1000) roland    (1000)    26799 2023-03-05 21:04:43.000000 scoop-template-engine-1.1.1/src/doc/markup.py
+-rw-------   0 roland    (1000) roland    (1000)   318974 2023-04-29 22:12:28.000000 scoop-template-engine-1.1.1/src/doc/scoop-prepare-bibtex-file.pdf
+-rw-------   0 roland    (1000) roland    (1000)   496041 2023-04-29 22:12:25.000000 scoop-template-engine-1.1.1/src/doc/scoop-template-engine.pdf
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.379385 scoop-template-engine-1.1.1/src/scoop_template_engine.egg-info/
+-rw-------   0 roland    (1000) roland    (1000)     2421 2023-04-29 22:15:00.000000 scoop-template-engine-1.1.1/src/scoop_template_engine.egg-info/PKG-INFO
+-rw-------   0 roland    (1000) roland    (1000)    62787 2023-04-29 22:15:00.000000 scoop-template-engine-1.1.1/src/scoop_template_engine.egg-info/SOURCES.txt
+-rw-------   0 roland    (1000) roland    (1000)        1 2023-04-29 22:15:00.000000 scoop-template-engine-1.1.1/src/scoop_template_engine.egg-info/dependency_links.txt
+-rw-------   0 roland    (1000) roland    (1000)       68 2023-04-29 22:15:00.000000 scoop-template-engine-1.1.1/src/scoop_template_engine.egg-info/entry_points.txt
+-rw-------   0 roland    (1000) roland    (1000)      158 2023-04-29 22:15:00.000000 scoop-template-engine-1.1.1/src/scoop_template_engine.egg-info/requires.txt
+-rw-------   0 roland    (1000) roland    (1000)       13 2023-04-29 22:15:00.000000 scoop-template-engine-1.1.1/src/scoop_template_engine.egg-info/top_level.txt
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.379385 scoop-template-engine-1.1.1/src/spbf/
+-rw-------   0 roland    (1000) roland    (1000)        0 2023-02-18 12:12:19.000000 scoop-template-engine-1.1.1/src/spbf/__init__.py
+-rw-------   0 roland    (1000) roland    (1000)    24233 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/spbf/__main__.py
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.379385 scoop-template-engine-1.1.1/src/ste/
+-rw-------   0 roland    (1000) roland    (1000)        0 2023-02-18 12:12:19.000000 scoop-template-engine-1.1.1/src/ste/__init__.py
+-rw-------   0 roland    (1000) roland    (1000)    29845 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/__main__.py
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.379385 scoop-template-engine-1.1.1/src/ste/manuscripts/
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.391385 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/
+-rwx------   0 roland    (1000) roland    (1000)     1011 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/init.py
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-aabmcb.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-aaembp.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-aaemcq.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-aamick.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-aanmf6.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-aapmcd.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-aastgj.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-abmcb8.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-abseba.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-acbcct.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-accacs.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-achre4.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-achsc5.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-acncdm.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-acsccc.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-acscii.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-acsodf.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-aeacb3.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-aeacc4.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-aeecco.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-aelccp.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-aesccq.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-aewcaa.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-afsthl.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-aidcbc.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-amacgu.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-amachv.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-amclct.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-amlccd.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-amlcef.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-amrcda.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-anaccx.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-ancac3.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-ancham.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-aoiab5.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-apaccd.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-apcach.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-apchd5.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-aptsfn.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-asbcd6.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-ascecg.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-ascefj.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-bcches.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-bichaw.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-bomaf6.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-cgdefu.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-chreay.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-cmatex.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-crtoec.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-enfuem.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-esthag.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-estlcu.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-iecred.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-inocaj.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-jaaucr.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-jacsat.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-jafcau.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-jamsef.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-jceaax.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-jceda8.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-jcisd8.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-jctcce.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-jmcmar.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-jnprdf.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-joceah.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-jpcafh.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-jpcbfk.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-jpccck.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-jpclcd.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-jprobs.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-langd5.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-mamobx.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-mpohbp.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-nalefd.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-oprdfk.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-orgnd7.sty
+-rw-------   0 roland    (1000) roland    (1000)     2419 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-orlef7.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-aabmcb.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-aaembp.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-aaemcq.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-aamick.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-aanmf6.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-aapmcd.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-aastgj.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-abmcb8.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-abseba.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-acbcct.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-accacs.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-achre4.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-achsc5.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-acncdm.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-acsccc.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-acscii.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-acsodf.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-aeacb3.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-aeacc4.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-aeecco.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-aelccp.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-aesccq.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-aewcaa.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-afsthl.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-aidcbc.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-amacgu.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-amachv.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-amclct.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-amlccd.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-amlcef.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-amrcda.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-anaccx.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-ancac3.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-ancham.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-aoiab5.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-apaccd.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-apcach.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-apchd5.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-aptsfn.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-asbcd6.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-ascecg.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-ascefj.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-bcches.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-bichaw.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-bomaf6.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-cgdefu.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-chreay.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-cmatex.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-crtoec.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-enfuem.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-esthag.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-estlcu.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-iecred.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-inocaj.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-jaaucr.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-jacsat.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-jafcau.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-jamsef.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-jceaax.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-jceda8.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-jcisd8.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-jctcce.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-jmcmar.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-jnprdf.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-joceah.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-jpcafh.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-jpcbfk.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-jpccck.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-jpclcd.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-jprobs.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-langd5.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-mamobx.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-mpohbp.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-nalefd.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-oprdfk.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-orgnd7.sty
+-rw-------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-orlef7.sty
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-aabmcb.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-aaembp.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-aaemcq.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-aamick.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-aanmf6.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-aapmcd.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-aastgj.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-abmcb8.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-abseba.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-acbcct.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-accacs.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-achre4.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-achsc5.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-acncdm.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-acsccc.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-acscii.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-acsodf.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-aeacb3.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-aeacc4.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-aeecco.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-aelccp.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-aesccq.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-aewcaa.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-afsthl.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-aidcbc.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-amacgu.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-amachv.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-amclct.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-amlccd.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-amlcef.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-amrcda.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-anaccx.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-ancac3.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-ancham.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-aoiab5.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-apaccd.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-apcach.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-apchd5.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-aptsfn.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-asbcd6.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-ascecg.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-ascefj.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-bcches.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-bichaw.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-bomaf6.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-cgdefu.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-chreay.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-cmatex.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-crtoec.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-enfuem.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-esthag.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-estlcu.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-iecred.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-inocaj.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-jaaucr.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-jacsat.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-jafcau.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-jamsef.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-jceaax.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-jceda8.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-jcisd8.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-jctcce.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-jmcmar.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-jnprdf.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-joceah.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-jpcafh.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-jpcbfk.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-jpccck.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-jpclcd.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-jprobs.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-langd5.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-mamobx.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-mpohbp.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-nalefd.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-oprdfk.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-orgnd7.tex
+-rw-------   0 roland    (1000) roland    (1000)    19067 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-orlef7.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.395385 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/
+-rwx------   0 roland    (1000) roland    (1000)      655 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/init.py
+-rw-------   0 roland    (1000) roland    (1000)     2561 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/postpreamble-amcomm.sty
+-rw-------   0 roland    (1000) roland    (1000)     2561 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/postpreamble-cpaa.sty
+-rw-------   0 roland    (1000) roland    (1000)     2561 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/postpreamble-dcds-b.sty
+-rw-------   0 roland    (1000) roland    (1000)     2561 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/postpreamble-dcds-s.sty
+-rw-------   0 roland    (1000) roland    (1000)     2561 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/postpreamble-dcds.sty
+-rw-------   0 roland    (1000) roland    (1000)     2561 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/postpreamble-eect.sty
+-rw-------   0 roland    (1000) roland    (1000)     2561 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/postpreamble-fods.sty
+-rw-------   0 roland    (1000) roland    (1000)     2561 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/postpreamble-ipi.sty
+-rw-------   0 roland    (1000) roland    (1000)     2561 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/postpreamble-jcd.sty
+-rw-------   0 roland    (1000) roland    (1000)     2561 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/postpreamble-jdg.sty
+-rw-------   0 roland    (1000) roland    (1000)     2561 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/postpreamble-jgm.sty
+-rw-------   0 roland    (1000) roland    (1000)     2561 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/postpreamble-jimo.sty
+-rw-------   0 roland    (1000) roland    (1000)     2561 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/postpreamble-krm.sty
+-rw-------   0 roland    (1000) roland    (1000)     2561 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/postpreamble-mcrf.sty
+-rw-------   0 roland    (1000) roland    (1000)     2561 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/postpreamble-mfc.sty
+-rw-------   0 roland    (1000) roland    (1000)     2561 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/postpreamble-naco.sty
+-rw-------   0 roland    (1000) roland    (1000)     2561 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/postpreamble-nhm.sty
+-rw-------   0 roland    (1000) roland    (1000)     4187 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/template-amcomm.tex
+-rw-------   0 roland    (1000) roland    (1000)     4187 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/template-cpaa.tex
+-rw-------   0 roland    (1000) roland    (1000)     4187 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/template-dcds-b.tex
+-rw-------   0 roland    (1000) roland    (1000)     4187 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/template-dcds-s.tex
+-rw-------   0 roland    (1000) roland    (1000)     4187 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/template-dcds.tex
+-rw-------   0 roland    (1000) roland    (1000)     4187 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/template-eect.tex
+-rw-------   0 roland    (1000) roland    (1000)     4187 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/template-fods.tex
+-rw-------   0 roland    (1000) roland    (1000)     4187 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/template-ipi.tex
+-rw-------   0 roland    (1000) roland    (1000)     4187 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/template-jcd.tex
+-rw-------   0 roland    (1000) roland    (1000)     4187 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/template-jdg.tex
+-rw-------   0 roland    (1000) roland    (1000)     4187 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/template-jgm.tex
+-rw-------   0 roland    (1000) roland    (1000)     4187 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/template-jimo.tex
+-rw-------   0 roland    (1000) roland    (1000)     4187 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/template-krm.tex
+-rw-------   0 roland    (1000) roland    (1000)     4187 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/template-mcrf.tex
+-rw-------   0 roland    (1000) roland    (1000)     4187 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/template-mfc.tex
+-rw-------   0 roland    (1000) roland    (1000)     4187 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/template-naco.tex
+-rw-------   0 roland    (1000) roland    (1000)     4187 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/template-nhm.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.375385 scoop-template-engine-1.1.1/src/ste/manuscripts/AMS/
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.395385 scoop-template-engine-1.1.1/src/ste/manuscripts/AMS/mcom/
+-rwx------   0 roland    (1000) roland    (1000)      984 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AMS/mcom/init.py
+-rw-------   0 roland    (1000) roland    (1000)     2401 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AMS/mcom/postpreamble-mcom.sty
+-rw-------   0 roland    (1000) roland    (1000)     1631 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/AMS/mcom/template-mcom.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.375385 scoop-template-engine-1.1.1/src/ste/manuscripts/Begell/
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.395385 scoop-template-engine-1.1.1/src/ste/manuscripts/Begell/ijuq/
+-rw-------   0 roland    (1000) roland    (1000)      324 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Begell/ijuq/IJ4UQ_Bibliography_Style.bst.patch
+-rwx------   0 roland    (1000) roland    (1000)     1326 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Begell/ijuq/init.py
+-rw-------   0 roland    (1000) roland    (1000)     2887 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Begell/ijuq/postpreamble-ijuq.sty
+-rw-------   0 roland    (1000) roland    (1000)     1271 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Begell/ijuq/preamble-ijuq.sty
+-rw-------   0 roland    (1000) roland    (1000)     2486 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Begell/ijuq/template-ijuq.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.375385 scoop-template-engine-1.1.1/src/ste/manuscripts/Centre Mersenne/
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.395385 scoop-template-engine-1.1.1/src/ste/manuscripts/Centre Mersenne/ojmo/
+-rwx------   0 roland    (1000) roland    (1000)      675 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Centre Mersenne/ojmo/init.py
+-rw-------   0 roland    (1000) roland    (1000)     2763 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Centre Mersenne/ojmo/postpreamble-ojmo.sty
+-rw-------   0 roland    (1000) roland    (1000)     1230 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Centre Mersenne/ojmo/preamble-ojmo.sty
+-rw-------   0 roland    (1000) roland    (1000)     1966 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Centre Mersenne/ojmo/template-ojmo.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.375385 scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.395385 scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/acvar/
+-rw-------   0 roland    (1000) roland    (1000)      699 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/acvar/init.py
+-rw-------   0 roland    (1000) roland    (1000)     2153 2023-04-29 10:06:57.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/acvar/postpreamble-acvar.sty
+-rw-------   0 roland    (1000) roland    (1000)     2525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/acvar/template-acvar.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.395385 scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/cmam/
+-rwx------   0 roland    (1000) roland    (1000)      711 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/cmam/init.py
+-rw-------   0 roland    (1000) roland    (1000)     2153 2023-04-29 10:06:57.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/cmam/postpreamble-cmam.sty
+-rw-------   0 roland    (1000) roland    (1000)     2525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/cmam/template-cmam.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.395385 scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/crelle/
+-rwx------   0 roland    (1000) roland    (1000)     1240 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/crelle/init.py
+-rw-------   0 roland    (1000) roland    (1000)     2574 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/crelle/postpreamble-crelle.sty
+-rw-------   0 roland    (1000) roland    (1000)     1262 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/crelle/preamble-crelle.sty
+-rw-------   0 roland    (1000) roland    (1000)     1194 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/crelle/prepreamble-crelle.sty
+-rw-------   0 roland    (1000) roland    (1000)     1771 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/crelle/template-crelle.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.395385 scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/jip/
+-rwx------   0 roland    (1000) roland    (1000)      707 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/jip/init.py
+-rw-------   0 roland    (1000) roland    (1000)     2153 2023-04-29 10:06:57.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/jip/postpreamble-jip.sty
+-rw-------   0 roland    (1000) roland    (1000)     2525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/jip/template-jip.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.395385 scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/jnm/
+-rwx------   0 roland    (1000) roland    (1000)      698 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/jnm/init.py
+-rw-------   0 roland    (1000) roland    (1000)     2153 2023-04-29 10:06:57.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/jnm/postpreamble-jnm.sty
+-rw-------   0 roland    (1000) roland    (1000)     2525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/jnm/template-jnm.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.375385 scoop-template-engine-1.1.1/src/ste/manuscripts/EMS/
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.395385 scoop-template-engine-1.1.1/src/ste/manuscripts/EMS/ag/
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/EMS/ag/postpreamble-ag.sty
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/EMS/ag/template-ag.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.395385 scoop-template-engine-1.1.1/src/ste/manuscripts/EMS/em/
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/EMS/em/postpreamble-em.sty
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/EMS/em/template-em.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.395385 scoop-template-engine-1.1.1/src/ste/manuscripts/EMS/rlm/
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/EMS/rlm/postpreamble-rlm.sty
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/EMS/rlm/template-rlm.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.375385 scoop-template-engine-1.1.1/src/ste/manuscripts/ESAIM/
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.395385 scoop-template-engine-1.1.1/src/ste/manuscripts/ESAIM/cocv/
+-rwx------   0 roland    (1000) roland    (1000)     1123 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ESAIM/cocv/init.py
+-rw-------   0 roland    (1000) roland    (1000)     2340 2023-04-29 10:01:35.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ESAIM/cocv/postpreamble-cocv.sty
+-rw-------   0 roland    (1000) roland    (1000)     1714 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ESAIM/cocv/template-cocv.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.395385 scoop-template-engine-1.1.1/src/ste/manuscripts/ESAIM/m2an/
+-rwx------   0 roland    (1000) roland    (1000)     1120 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ESAIM/m2an/init.py
+-rw-------   0 roland    (1000) roland    (1000)     2340 2023-04-29 10:01:30.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ESAIM/m2an/postpreamble-m2an.sty
+-rw-------   0 roland    (1000) roland    (1000)     1708 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/ESAIM/m2an/template-m2an.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.375385 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.419385 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/
+-rwx------   0 roland    (1000) roland    (1000)     1604 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/init.py
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-aam.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-acha.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-advengsoft.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-aim.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-amc.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-aml.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-apal.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-apm.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-apnum.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-arcontrol.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-array.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-bcra.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-bdr.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-bica.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-brain.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-bulsci.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-cad.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-cam.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-camwa.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-chaos.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-cma.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-cnsns.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-cocom.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-coisb.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-cola.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-comgeo.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-commatsci.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-compgeo.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-compstruc.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-conengprac.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-cosrev.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-cpc.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-csda.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-csfx.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-csl.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-dajour.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-dam.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-dark.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-difgeo.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-disc.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-disopt.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ecocom.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ecolmodel.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ecosta.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ejc.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ejor.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-enganabound.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-engappai.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-exco.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-exmath.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ffa.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-finel.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-fss.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-geb.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-geomphys.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-gmod.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-hcc.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-health.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-heliyon.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ic.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ijforecast.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ime.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-indag.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ins.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ipl.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jaca.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jalgebra.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jat.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jcmds.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jco.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jcp.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jcpx.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jcss.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jcta.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jctb.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jde.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jebo.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jeconom.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jedc.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jet.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jfa.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jfranklin.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jlamp.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jmaa.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jmateco.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jnt.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jocsci.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jpaa.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jprocont.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jspi.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jsymbc.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-laa.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-matcom.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-matpur.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-mbs.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-mlwa.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-mss.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-na.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-nahs.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-nanocomnet.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-neunet.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-nlm.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-nonrwa.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-nppp.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-nuclphysb.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-orl.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-padiff.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-patterns.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-physa.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-physd.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-physleta.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-physletb.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-plrev.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-pmc.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-pr.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-red.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-rico.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-rinam.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-sasc.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-spa.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-spasta.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-stapro.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-swevo.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-sysconle.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-tcs.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-topol.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-vehcom.sty
+-rw-------   0 roland    (1000) roland    (1000)     2275 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-wace.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-aam.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-acha.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-advengsoft.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-aim.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-amc.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-aml.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-apal.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-apm.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-apnum.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-arcontrol.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-array.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-bcra.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-bdr.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-bica.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-brain.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-bulsci.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-cad.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-cam.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-camwa.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-chaos.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-cma.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-cnsns.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-cocom.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-coisb.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-cola.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-comgeo.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-commatsci.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-compgeo.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-compstruc.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-conengprac.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-cosrev.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-cpc.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-csda.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-csfx.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-csl.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-dajour.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-dam.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-dark.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-difgeo.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-disc.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-disopt.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ecocom.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ecolmodel.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ecosta.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ejc.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ejor.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-enganabound.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-engappai.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-exco.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-exmath.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ffa.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-finel.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-fss.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-geb.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-geomphys.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-gmod.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-hcc.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-health.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-heliyon.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ic.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ijforecast.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ime.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-indag.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ins.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ipl.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jaca.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jalgebra.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jat.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jcmds.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jco.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jcp.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jcpx.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jcss.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jcta.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jctb.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jde.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jebo.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jeconom.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jedc.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jet.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jfa.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jfranklin.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jlamp.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jmaa.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jmateco.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jnt.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jocsci.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jpaa.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jprocont.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jspi.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jsymbc.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-laa.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-matcom.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-matpur.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-mbs.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-mlwa.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-mss.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-na.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-nahs.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-nanocomnet.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-neunet.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-nlm.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-nonrwa.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-nppp.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-nuclphysb.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-orl.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-padiff.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-patterns.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-physa.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-physd.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-physleta.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-physletb.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-plrev.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-pmc.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-pr.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-red.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-rico.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-rinam.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-sasc.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-spa.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-spasta.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-stapro.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-swevo.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-sysconle.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-tcs.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-topol.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-vehcom.sty
+-rw-------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-wace.sty
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-aam.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-acha.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-advengsoft.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-aim.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-amc.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-aml.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-apal.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-apm.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-apnum.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-arcontrol.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-array.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-bcra.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-bdr.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-bica.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-brain.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-bulsci.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-cad.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-cam.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-camwa.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-chaos.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-cma.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-cnsns.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-cocom.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-coisb.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-cola.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-comgeo.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-commatsci.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-compgeo.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-compstruc.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-conengprac.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-cosrev.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-cpc.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-csda.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-csfx.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-csl.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-dajour.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-dam.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-dark.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-difgeo.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-disc.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-disopt.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ecocom.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ecolmodel.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ecosta.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ejc.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ejor.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-enganabound.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-engappai.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-exco.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-exmath.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ffa.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-finel.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-fss.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-geb.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-geomphys.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-gmod.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-hcc.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-health.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-heliyon.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ic.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ijforecast.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ime.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-indag.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ins.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ipl.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jaca.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jalgebra.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jat.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jcmds.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jco.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jcp.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jcpx.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jcss.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jcta.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jctb.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jde.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jebo.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jeconom.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jedc.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jet.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jfa.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jfranklin.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jlamp.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jmaa.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jmateco.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jnt.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jocsci.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jpaa.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jprocont.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jspi.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jsymbc.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-laa.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-matcom.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-matpur.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-mbs.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-mlwa.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-mss.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-na.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-nahs.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-nanocomnet.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-neunet.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-nlm.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-nonrwa.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-nppp.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-nuclphysb.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-orl.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-padiff.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-patterns.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-physa.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-physd.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-physleta.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-physletb.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-plrev.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-pmc.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-pr.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-red.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-rico.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-rinam.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-sasc.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-spa.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-spasta.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-stapro.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-swevo.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-sysconle.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-tcs.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-topol.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-vehcom.tex
+-rw-------   0 roland    (1000) roland    (1000)    23355 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-wace.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.419385 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/ifac/
+-rwx------   0 roland    (1000) roland    (1000)      788 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/ifac/init.py
+-rw-------   0 roland    (1000) roland    (1000)     2998 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/ifac/postpreamble-ifac.sty
+-rw-------   0 roland    (1000) roland    (1000)     1307 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/ifac/preamble-ifac.sty
+-rw-------   0 roland    (1000) roland    (1000)     1851 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/ifac/template-ifac.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.419385 scoop-template-engine-1.1.1/src/ste/manuscripts/Frontiers/
+-rwx------   0 roland    (1000) roland    (1000)      706 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Frontiers/init.py
+-rw-------   0 roland    (1000) roland    (1000)     2812 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Frontiers/postpreamble-fams.sty
+-rw-------   0 roland    (1000) roland    (1000)     2404 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Frontiers/template-fams.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.427385 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/
+-rw-------   0 roland    (1000) roland    (1000)     1093 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/init.py
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-bbiici.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-bioffn.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-bmbucs.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-bpeeae.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-cqgrdg.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-dmatb7.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-ejphd4.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-ejssbg.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-erc.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-ercl.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-ere.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-erenbl.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-erh.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-erisal.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-erlnal.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-esltac.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-fcsuah.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-fpelab.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-ijemkf.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-ip.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-isoccm.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-jbrobw.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-jcapbp.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-jcomel.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-jionas.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-jmmiez.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-jneiez.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-joopca.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-jpamb5.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-jpapbe.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-jpapeh.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-jpcofp.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-jpcogq.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-jpeoey.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-jpgped.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-jpmoc4.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-jppokr.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-jrprea.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-jsmtc6.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-mafeb2.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-mlstck.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-mmuabd.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-mqtaaz.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-mreac3.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-msmeeu.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-mstcep.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-mtrgau.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-nceecn.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-neaxa4.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-nfaub3.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-njopfm.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-nnoter.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-nonle5.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-nufuau.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-pberb8.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-pbhiat.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-perndg.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-pheda7.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-phmba7.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-phstbo.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-pmeae3.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-ppcfet.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-prelcz.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-psteeu.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-qstuah.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-rpphag.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-smster.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-ssteet.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-stmpcw.sty
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-sustef.sty
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-bbiici.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-bioffn.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-bmbucs.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-bpeeae.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-cqgrdg.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-dmatb7.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-ejphd4.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-ejssbg.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-erc.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-ercl.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-ere.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-erenbl.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-erh.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-erisal.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-erlnal.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-esltac.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-fcsuah.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-fpelab.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-ijemkf.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-ip.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-isoccm.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-jbrobw.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-jcapbp.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-jcomel.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-jionas.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-jmmiez.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-jneiez.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-joopca.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-jpamb5.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-jpapbe.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-jpapeh.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-jpcofp.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-jpcogq.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-jpeoey.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-jpgped.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-jpmoc4.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-jppokr.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-jrprea.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-jsmtc6.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-mafeb2.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-mlstck.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-mmuabd.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-mqtaaz.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-mreac3.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-msmeeu.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-mstcep.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-mtrgau.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-nceecn.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-neaxa4.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-nfaub3.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-njopfm.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-nnoter.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-nonle5.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-nufuau.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-pberb8.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-pbhiat.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-perndg.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-pheda7.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-phmba7.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-phstbo.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-pmeae3.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-ppcfet.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-prelcz.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-psteeu.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-qstuah.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-rpphag.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-smster.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-ssteet.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-stmpcw.tex
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-sustef.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.375385 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.431385 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/
+-r--------   0 roland    (1000) roland    (1000)     2449 2023-04-29 22:13:07.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-aa.sty
+-r--------   0 roland    (1000) roland    (1000)     2599 2023-04-29 22:13:07.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-acdm.sty
+-r--------   0 roland    (1000) roland    (1000)     2247 2023-04-29 22:13:07.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-amspreprint.sty
+-r--------   0 roland    (1000) roland    (1000)     2773 2023-04-29 22:13:07.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-bit.sty
+-r--------   0 roland    (1000) roland    (1000)     2275 2023-04-29 22:13:07.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-cma.sty
+-r--------   0 roland    (1000) roland    (1000)     2153 2023-04-29 22:13:07.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-cmam.sty
+-r--------   0 roland    (1000) roland    (1000)     2340 2023-04-29 22:13:07.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-cocv.sty
+-r--------   0 roland    (1000) roland    (1000)     2574 2023-04-29 22:13:07.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-crelle.sty
+-r--------   0 roland    (1000) roland    (1000)     3154 2023-04-29 22:13:08.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-etna.sty
+-r--------   0 roland    (1000) roland    (1000)     2812 2023-04-29 22:13:08.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-fams.sty
+-r--------   0 roland    (1000) roland    (1000)     2417 2023-04-29 22:13:11.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-gamm.sty
+-r--------   0 roland    (1000) roland    (1000)     2419 2023-04-29 22:13:11.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-iecred.sty
+-r--------   0 roland    (1000) roland    (1000)     2998 2023-04-29 22:13:11.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-ifac.sty
+-r--------   0 roland    (1000) roland    (1000)     2490 2023-04-29 22:13:11.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-ijcga.sty
+-r--------   0 roland    (1000) roland    (1000)     3231 2023-04-29 22:13:11.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-ijcm.sty
+-r--------   0 roland    (1000) roland    (1000)     2887 2023-04-29 22:13:11.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-ijuq.sty
+-r--------   0 roland    (1000) roland    (1000)     2302 2023-04-29 22:13:12.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-imanum.sty
+-r--------   0 roland    (1000) roland    (1000)     2276 2023-04-29 22:13:12.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-jmiv.sty
+-r--------   0 roland    (1000) roland    (1000)     1976 2023-04-29 22:13:15.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-jnsao.sty
+-r--------   0 roland    (1000) roland    (1000)     2774 2023-04-29 22:13:15.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-jota.sty
+-r--------   0 roland    (1000) roland    (1000)     2773 2023-04-29 22:13:15.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-jsc.sty
+-r--------   0 roland    (1000) roland    (1000)     2340 2023-04-29 22:13:15.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-m2an.sty
+-r--------   0 roland    (1000) roland    (1000)     2498 2023-04-29 22:13:16.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-m3as.sty
+-r--------   0 roland    (1000) roland    (1000)     2401 2023-04-29 22:13:16.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-mcom.sty
+-r--------   0 roland    (1000) roland    (1000)     2561 2023-04-29 22:13:16.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-mcrf.sty
+-r--------   0 roland    (1000) roland    (1000)     2050 2023-04-29 22:13:17.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-mma.sty
+-r--------   0 roland    (1000) roland    (1000)     2050 2023-04-29 22:13:20.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-nla.sty
+-r--------   0 roland    (1000) roland    (1000)     2050 2023-04-29 22:13:20.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-nme.sty
+-r--------   0 roland    (1000) roland    (1000)     2763 2023-04-29 22:13:20.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-ojmo.sty
+-r--------   0 roland    (1000) roland    (1000)     2582 2023-04-29 22:13:20.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-opt.sty
+-r--------   0 roland    (1000) roland    (1000)     3007 2023-04-29 22:13:20.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-pamm.sty
+-r--------   0 roland    (1000) roland    (1000)     2497 2023-04-29 22:13:20.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-ppl.sty
+-r--------   0 roland    (1000) roland    (1000)     2219 2023-04-29 22:13:21.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-siims.sty
+-r--------   0 roland    (1000) roland    (1000)     2219 2023-04-29 22:13:21.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-siopt.sty
+-r--------   0 roland    (1000) roland    (1000)     2417 2023-04-29 22:13:24.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-zamm.sty
+-r--------   0 roland    (1000) roland    (1000)     1345 2023-04-29 22:13:07.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/preamble-acdm.sty
+-r--------   0 roland    (1000) roland    (1000)     1113 2023-04-29 22:13:07.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/preamble-bit.sty
+-r--------   0 roland    (1000) roland    (1000)     1262 2023-04-29 22:13:07.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/preamble-crelle.sty
+-r--------   0 roland    (1000) roland    (1000)     1307 2023-04-29 22:13:11.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/preamble-ifac.sty
+-r--------   0 roland    (1000) roland    (1000)     1340 2023-04-29 22:13:11.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/preamble-ijcm.sty
+-r--------   0 roland    (1000) roland    (1000)     1271 2023-04-29 22:13:11.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/preamble-ijuq.sty
+-r--------   0 roland    (1000) roland    (1000)     1115 2023-04-29 22:13:12.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/preamble-jmiv.sty
+-r--------   0 roland    (1000) roland    (1000)     1114 2023-04-29 22:13:15.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/preamble-jota.sty
+-r--------   0 roland    (1000) roland    (1000)     1113 2023-04-29 22:13:15.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/preamble-jsc.sty
+-r--------   0 roland    (1000) roland    (1000)     1230 2023-04-29 22:13:20.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/preamble-ojmo.sty
+-r--------   0 roland    (1000) roland    (1000)     1117 2023-04-29 22:13:07.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/prepreamble-cma.sty
+-r--------   0 roland    (1000) roland    (1000)     1194 2023-04-29 22:13:07.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/prepreamble-crelle.sty
+-r--------   0 roland    (1000) roland    (1000)     1116 2023-04-29 22:13:08.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/prepreamble-etna.sty
+-r--------   0 roland    (1000) roland    (1000)     1193 2023-04-29 22:13:11.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/prepreamble-iecred.sty
+-r--------   0 roland    (1000) roland    (1000)     1250 2023-04-29 22:13:12.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/prepreamble-imanum.sty
+-r--------   0 roland    (1000) roland    (1000)     1525 2023-04-29 22:13:12.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/prepreamble-jmiv.sty
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.375385 scoop-template-engine-1.1.1/src/ste/manuscripts/Oxford Academic/
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.431385 scoop-template-engine-1.1.1/src/ste/manuscripts/Oxford Academic/imanum/
+-rwx------   0 roland    (1000) roland    (1000)      923 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Oxford Academic/imanum/init.py
+-rw-------   0 roland    (1000) roland    (1000)     2302 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Oxford Academic/imanum/postpreamble-imanum.sty
+-rw-------   0 roland    (1000) roland    (1000)     1250 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Oxford Academic/imanum/prepreamble-imanum.sty
+-rw-------   0 roland    (1000) roland    (1000)     2325 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Oxford Academic/imanum/template-imanum.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.431385 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/
+-rwx------   0 roland    (1000) roland    (1000)      812 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/init.py
+-rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/postpreamble-mms.sty
+-rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/postpreamble-siap.sty
+-rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/postpreamble-sicomp.sty
+-rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/postpreamble-sicon.sty
+-rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/postpreamble-sidma.sty
+-rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/postpreamble-sima.sty
+-rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/postpreamble-simax.sty
+-rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/postpreamble-sinum.sty
+-rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/postpreamble-siopt.sty
+-rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/postpreamble-sirev.sty
+-rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/postpreamble-sisc.sty
+-rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/postpreamble-tvp.sty
+-rw-------   0 roland    (1000) roland    (1000)     3236 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/template-mms.tex
+-rw-------   0 roland    (1000) roland    (1000)     3236 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/template-siap.tex
+-rw-------   0 roland    (1000) roland    (1000)     3236 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/template-sicomp.tex
+-rw-------   0 roland    (1000) roland    (1000)     3236 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/template-sicon.tex
+-rw-------   0 roland    (1000) roland    (1000)     3236 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/template-sidma.tex
+-rw-------   0 roland    (1000) roland    (1000)     3236 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/template-sima.tex
+-rw-------   0 roland    (1000) roland    (1000)     3236 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/template-simax.tex
+-rw-------   0 roland    (1000) roland    (1000)     3236 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/template-sinum.tex
+-rw-------   0 roland    (1000) roland    (1000)     3236 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/template-siopt.tex
+-rw-------   0 roland    (1000) roland    (1000)     3236 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/template-sirev.tex
+-rw-------   0 roland    (1000) roland    (1000)     3236 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/template-sisc.tex
+-rw-------   0 roland    (1000) roland    (1000)     3236 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/template-tvp.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.431385 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAMOnline/
+-rwx------   0 roland    (1000) roland    (1000)      814 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAMOnline/init.py
+-rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAMOnline/postpreamble-juq.sty
+-rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAMOnline/postpreamble-siads.sty
+-rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAMOnline/postpreamble-siaga.sty
+-rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAMOnline/postpreamble-sifin.sty
+-rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAMOnline/postpreamble-siims.sty
+-rw-------   0 roland    (1000) roland    (1000)     2219 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAMOnline/postpreamble-simods.sty
+-rw-------   0 roland    (1000) roland    (1000)     2595 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAMOnline/template-juq.tex
+-rw-------   0 roland    (1000) roland    (1000)     2595 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAMOnline/template-siads.tex
+-rw-------   0 roland    (1000) roland    (1000)     2595 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAMOnline/template-siaga.tex
+-rw-------   0 roland    (1000) roland    (1000)     2595 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAMOnline/template-sifin.tex
+-rw-------   0 roland    (1000) roland    (1000)     2595 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAMOnline/template-siims.tex
+-rw-------   0 roland    (1000) roland    (1000)     2595 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/SIAMOnline/template-simods.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.375385 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.431385 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bit/
+-rw-------   0 roland    (1000) roland    (1000)     1321 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bit/init.py
+-rw-------   0 roland    (1000) roland    (1000)     2773 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bit/postpreamble-bit.sty
+-rw-------   0 roland    (1000) roland    (1000)     1113 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bit/preamble-bit.sty
+-rw-------   0 roland    (1000) roland    (1000)     2221 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bit/template-bit.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.435385 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bmcart.cls/
+-rw-------   0 roland    (1000) roland    (1000)      864 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bmcart.cls/init.py
+-rw-------   0 roland    (1000) roland    (1000)     2599 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bmcart.cls/postpreamble-acdm.sty
+-rw-------   0 roland    (1000) roland    (1000)     2599 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bmcart.cls/postpreamble-bvp.sty
+-rw-------   0 roland    (1000) roland    (1000)     2599 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bmcart.cls/postpreamble-jia.sty
+-rw-------   0 roland    (1000) roland    (1000)     2599 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bmcart.cls/postpreamble-jmi.sty
+-rw-------   0 roland    (1000) roland    (1000)     1345 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bmcart.cls/preamble-acdm.sty
+-rw-------   0 roland    (1000) roland    (1000)     1345 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bmcart.cls/preamble-bvp.sty
+-rw-------   0 roland    (1000) roland    (1000)     1345 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bmcart.cls/preamble-jia.sty
+-rw-------   0 roland    (1000) roland    (1000)     1345 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bmcart.cls/preamble-jmi.sty
+-rw-------   0 roland    (1000) roland    (1000)     2353 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bmcart.cls/template-acdm.tex
+-rw-------   0 roland    (1000) roland    (1000)     2353 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bmcart.cls/template-bvp.tex
+-rw-------   0 roland    (1000) roland    (1000)     2353 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bmcart.cls/template-jia.tex
+-rw-------   0 roland    (1000) roland    (1000)     2353 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bmcart.cls/template-jmi.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.435385 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/jota/
+-rw-------   0 roland    (1000) roland    (1000)      955 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/jota/init.py
+-rw-------   0 roland    (1000) roland    (1000)     2774 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/jota/postpreamble-jota.sty
+-rw-------   0 roland    (1000) roland    (1000)     1114 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/jota/preamble-jota.sty
+-rw-------   0 roland    (1000) roland    (1000)     2148 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/jota/template-jota.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.439385 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/
+-rw-------   0 roland    (1000) roland    (1000)      847 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/init.py
+-rw-------   0 roland    (1000) roland    (1000)     2276 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-acom.sty
+-rw-------   0 roland    (1000) roland    (1000)     2276 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-amo.sty
+-rw-------   0 roland    (1000) roland    (1000)     2276 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-calcolo.sty
+-rw-------   0 roland    (1000) roland    (1000)     2276 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-camcos.sty
+-rw-------   0 roland    (1000) roland    (1000)     2276 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-cm.sty
+-rw-------   0 roland    (1000) roland    (1000)     2276 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-coam.sty
+-rw-------   0 roland    (1000) roland    (1000)     2276 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-coap.sty
+-rw-------   0 roland    (1000) roland    (1000)     2276 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-cvpde.sty
+-rw-------   0 roland    (1000) roland    (1000)     2276 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-dcg.sty
+-rw-------   0 roland    (1000) roland    (1000)     2276 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-focm.sty
+-rw-------   0 roland    (1000) roland    (1000)     2276 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-ijot.sty
+-rw-------   0 roland    (1000) roland    (1000)     2276 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-inge.sty
+-rw-------   0 roland    (1000) roland    (1000)     2276 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-jmiv.sty
+-rw-------   0 roland    (1000) roland    (1000)     2276 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-jogo.sty
+-rw-------   0 roland    (1000) roland    (1000)     2276 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-maana.sty
+-rw-------   0 roland    (1000) roland    (1000)     2276 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-mathbio.sty
+-rw-------   0 roland    (1000) roland    (1000)     2276 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-mathprog.sty
+-rw-------   0 roland    (1000) roland    (1000)     2276 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-mmor.sty
+-rw-------   0 roland    (1000) roland    (1000)     2276 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-ms.sty
+-rw-------   0 roland    (1000) roland    (1000)     2276 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-numa.sty
+-rw-------   0 roland    (1000) roland    (1000)     2276 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-numalg.sty
+-rw-------   0 roland    (1000) roland    (1000)     2276 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-pdea.sty
+-rw-------   0 roland    (1000) roland    (1000)     2276 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-rm.sty
+-rw-------   0 roland    (1000) roland    (1000)     2276 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-svva.sty
+-rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-acom.sty
+-rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-amo.sty
+-rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-calcolo.sty
+-rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-camcos.sty
+-rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-cm.sty
+-rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-coam.sty
+-rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-coap.sty
+-rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-cvpde.sty
+-rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-dcg.sty
+-rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-focm.sty
+-rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-ijot.sty
+-rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-inge.sty
+-rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-jmiv.sty
+-rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-jogo.sty
+-rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-maana.sty
+-rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-mathbio.sty
+-rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-mathprog.sty
+-rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-mmor.sty
+-rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-ms.sty
+-rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-numa.sty
+-rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-numalg.sty
+-rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-pdea.sty
+-rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-rm.sty
+-rw-------   0 roland    (1000) roland    (1000)     1115 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-svva.sty
+-rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-acom.sty
+-rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-amo.sty
+-rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-calcolo.sty
+-rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-camcos.sty
+-rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-cm.sty
+-rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-coam.sty
+-rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-coap.sty
+-rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-cvpde.sty
+-rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-dcg.sty
+-rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-focm.sty
+-rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-ijot.sty
+-rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-inge.sty
+-rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-jmiv.sty
+-rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-jogo.sty
+-rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-maana.sty
+-rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-mathbio.sty
+-rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-mathprog.sty
+-rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-mmor.sty
+-rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-ms.sty
+-rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-numa.sty
+-rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-numalg.sty
+-rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-pdea.sty
+-rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-rm.sty
+-rw-------   0 roland    (1000) roland    (1000)     1525 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-svva.sty
+-rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-acom.tex
+-rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-amo.tex
+-rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-calcolo.tex
+-rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-camcos.tex
+-rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-cm.tex
+-rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-coam.tex
+-rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-coap.tex
+-rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-cvpde.tex
+-rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-dcg.tex
+-rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-focm.tex
+-rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-ijot.tex
+-rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-inge.tex
+-rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-jmiv.tex
+-rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-jogo.tex
+-rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-maana.tex
+-rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-mathbio.tex
+-rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-mathprog.tex
+-rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-mmor.tex
+-rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-ms.tex
+-rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-numa.tex
+-rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-numalg.tex
+-rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-pdea.tex
+-rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-rm.tex
+-rw-------   0 roland    (1000) roland    (1000)     6662 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-svva.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.439385 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/svjour3.cls/
+-rw-------   0 roland    (1000) roland    (1000)      744 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/svjour3.cls/init.py
+-rw-------   0 roland    (1000) roland    (1000)     2773 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/svjour3.cls/postpreamble-jsc.sty
+-rw-------   0 roland    (1000) roland    (1000)     2773 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/svjour3.cls/postpreamble-mpc.sty
+-rw-------   0 roland    (1000) roland    (1000)     2773 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/svjour3.cls/postpreamble-opte.sty
+-rw-------   0 roland    (1000) roland    (1000)     1113 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/svjour3.cls/preamble-jsc.sty
+-rw-------   0 roland    (1000) roland    (1000)     1113 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/svjour3.cls/preamble-mpc.sty
+-rw-------   0 roland    (1000) roland    (1000)     1113 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/svjour3.cls/preamble-opte.sty
+-rw-------   0 roland    (1000) roland    (1000)     2436 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/svjour3.cls/template-jsc.tex
+-rw-------   0 roland    (1000) roland    (1000)     2436 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/svjour3.cls/template-mpc.tex
+-rw-------   0 roland    (1000) roland    (1000)     2436 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/svjour3.cls/template-opte.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.439385 scoop-template-engine-1.1.1/src/ste/manuscripts/TaylorAndFrancis/
+-rwx------   0 roland    (1000) roland    (1000)      806 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/TaylorAndFrancis/init.py
+-rw-------   0 roland    (1000) roland    (1000)     2582 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/TaylorAndFrancis/postpreamble-apa.sty
+-rw-------   0 roland    (1000) roland    (1000)     2582 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/TaylorAndFrancis/postpreamble-eno.sty
+-rw-------   0 roland    (1000) roland    (1000)     2582 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/TaylorAndFrancis/postpreamble-oms.sty
+-rw-------   0 roland    (1000) roland    (1000)     2582 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/TaylorAndFrancis/postpreamble-opt.sty
+-rw-------   0 roland    (1000) roland    (1000)     2353 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/TaylorAndFrancis/template-apa.tex
+-rw-------   0 roland    (1000) roland    (1000)     2353 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/TaylorAndFrancis/template-eno.tex
+-rw-------   0 roland    (1000) roland    (1000)     2353 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/TaylorAndFrancis/template-oms.tex
+-rw-------   0 roland    (1000) roland    (1000)     2353 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/TaylorAndFrancis/template-opt.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.375385 scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.439385 scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/gamm/
+-rwx------   0 roland    (1000) roland    (1000)     1596 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/gamm/init.py
+-rw-------   0 roland    (1000) roland    (1000)     2417 2023-04-29 10:00:32.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/gamm/postpreamble-gamm.sty
+-rw-------   0 roland    (1000) roland    (1000)     2041 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/gamm/template-gamm.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.439385 scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/mma/
+-rwx------   0 roland    (1000) roland    (1000)     2197 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/mma/init.py
+-rw-------   0 roland    (1000) roland    (1000)     2050 2023-04-29 10:00:42.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/mma/postpreamble-mma.sty
+-rw-------   0 roland    (1000) roland    (1000)     2405 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/mma/template-mma.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.439385 scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/nla/
+-rwx------   0 roland    (1000) roland    (1000)     2125 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/nla/init.py
+-rw-------   0 roland    (1000) roland    (1000)     2050 2023-04-29 10:00:54.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/nla/postpreamble-nla.sty
+-rw-------   0 roland    (1000) roland    (1000)     2011 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/nla/template-nla.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.439385 scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/nme/
+-rwx------   0 roland    (1000) roland    (1000)     2207 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/nme/init.py
+-rw-------   0 roland    (1000) roland    (1000)     2050 2023-04-29 10:00:37.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/nme/postpreamble-nme.sty
+-rw-------   0 roland    (1000) roland    (1000)     2433 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/nme/template-nme.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.439385 scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/pamm/
+-rwx------   0 roland    (1000) roland    (1000)      732 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/pamm/init.py
+-rw-------   0 roland    (1000) roland    (1000)     3007 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/pamm/postpreamble-pamm.sty
+-rw-------   0 roland    (1000) roland    (1000)     1871 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/pamm/template-pamm.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.439385 scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/zamm/
+-rwx------   0 roland    (1000) roland    (1000)     1640 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/zamm/init.py
+-rw-------   0 roland    (1000) roland    (1000)     2417 2023-04-29 10:00:28.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/zamm/postpreamble-zamm.sty
+-rw-------   0 roland    (1000) roland    (1000)     2019 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/zamm/template-zamm.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.375385 scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.439385 scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/aa/
+-rwx------   0 roland    (1000) roland    (1000)      930 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/aa/init.py
+-rw-------   0 roland    (1000) roland    (1000)     2449 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/aa/postpreamble-aa.sty
+-rw-------   0 roland    (1000) roland    (1000)     1980 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/aa/template-aa.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.439385 scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/ijcga/
+-rwx------   0 roland    (1000) roland    (1000)      831 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/ijcga/init.py
+-rw-------   0 roland    (1000) roland    (1000)     2490 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/ijcga/postpreamble-ijcga.sty
+-rw-------   0 roland    (1000) roland    (1000)     1966 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/ijcga/template-ijcga.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.439385 scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/ijcm/
+-rwx------   0 roland    (1000) roland    (1000)      810 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/ijcm/init.py
+-rw-------   0 roland    (1000) roland    (1000)     3231 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/ijcm/postpreamble-ijcm.sty
+-rw-------   0 roland    (1000) roland    (1000)     1340 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/ijcm/preamble-ijcm.sty
+-rw-------   0 roland    (1000) roland    (1000)     2023 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/ijcm/template-ijcm.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.443385 scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/m3as/
+-rwx------   0 roland    (1000) roland    (1000)      815 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/m3as/init.py
+-rw-------   0 roland    (1000) roland    (1000)     2498 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/m3as/postpreamble-m3as.sty
+-rw-------   0 roland    (1000) roland    (1000)     2065 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/m3as/template-m3as.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.443385 scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/ppl/
+-rwx------   0 roland    (1000) roland    (1000)     1221 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/ppl/init.py
+-rw-------   0 roland    (1000) roland    (1000)     2497 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/ppl/postpreamble-ppl.sty
+-rw-------   0 roland    (1000) roland    (1000)     2155 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/ppl/template-ppl.tex
+-rw-------   0 roland    (1000) roland    (1000)     1340 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/ppl/ws-ppl.bst.patch
+-rw-------   0 roland    (1000) roland    (1000)        0 2023-02-18 12:12:19.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/__init__.py
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.443385 scoop-template-engine-1.1.1/src/ste/manuscripts/etna/
+-rw-------   0 roland    (1000) roland    (1000)     2773 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/etna/etna.cls.patch
+-rwx------   0 roland    (1000) roland    (1000)     1685 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/etna/init.py
+-rw-------   0 roland    (1000) roland    (1000)     3154 2023-04-29 22:09:22.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/etna/postpreamble-etna.sty
+-rw-------   0 roland    (1000) roland    (1000)     1116 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/etna/prepreamble-etna.sty
+-rw-------   0 roland    (1000) roland    (1000)     2111 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/etna/template-etna.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.443385 scoop-template-engine-1.1.1/src/ste/manuscripts/jnsao/
+-rwx------   0 roland    (1000) roland    (1000)      661 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/jnsao/init.py
+-rw-------   0 roland    (1000) roland    (1000)     1976 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/jnsao/postpreamble-jnsao.sty
+-rw-------   0 roland    (1000) roland    (1000)     1678 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/jnsao/template-jnsao.tex
+-rw-------   0 roland    (1000) roland    (1000)   107629 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/manuscripts.py
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.443385 scoop-template-engine-1.1.1/src/ste/manuscripts/scoop/
+-rw-------   0 roland    (1000) roland    (1000)     2247 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/scoop/postpreamble-amspreprint.sty
+-rw-------   0 roland    (1000) roland    (1000)    10720 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/scoop/template-amspreprint.tex
+-rw-------   0 roland    (1000) roland    (1000)      520 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/manuscripts/scoop/template-bibgenerator.tex
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.375385 scoop-template-engine-1.1.1/src/ste/schemes/
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.443385 scoop-template-engine-1.1.1/src/ste/schemes/manuscript/
+-rw-------   0 roland    (1000) roland    (1000)      132 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/schemes/manuscript/abstract.tex
+-rw-------   0 roland    (1000) roland    (1000)      213 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/schemes/manuscript/content.tex
+-rw-------   0 roland    (1000) roland    (1000)      388 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/schemes/manuscript/manuscript.bib
+-rw-------   0 roland    (1000) roland    (1000)       73 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/schemes/manuscript/manuscript.sty
+-rw-------   0 roland    (1000) roland    (1000)     1433 2023-04-29 10:30:46.000000 scoop-template-engine-1.1.1/src/ste/schemes/manuscript/manuscript.yaml
+drwx------   0 roland    (1000) roland    (1000)        0 2023-04-29 22:15:00.443385 scoop-template-engine-1.1.1/src/ste/utilities/
+-rw-------   0 roland    (1000) roland    (1000)        0 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/utilities/__init__.py
+-rw-------   0 roland    (1000) roland    (1000)     9510 2023-04-01 21:10:27.000000 scoop-template-engine-1.1.1/src/ste/utilities/utilities.py
```

### Comparing `scoop-template-engine-1.1.0/CHANGELOG.md` & `scoop-template-engine-1.1.1/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
+### Changed
+- Review and amend documentation.
 
 ## [1.1.0] - 2023-04-29
 ### Added
 - Add `orcid:` key to `authors:`.
 ### Changed
 - Implement `--protectfamilynames` switch into `spbf`.
```

### Comparing `scoop-template-engine-1.1.0/DESCRIPTION.md` & `scoop-template-engine-1.1.1/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/LICENSE` & `scoop-template-engine-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/MANIFEST.in` & `scoop-template-engine-1.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/PKG-INFO` & `scoop-template-engine-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoop-template-engine
-Version: 1.1.0
+Version: 1.1.1
 Summary: Prepare manuscripts in LaTeX
 Author-email: Roland Herzog <roland.herzog@iwr.uni-heidelberg.de>
 Project-URL: homepage, https://gitlab.com/scoopgroup-public/scoop-template-engine
 Project-URL: repository, https://gitlab.com/scoopgroup-public/scoop-template-engine
 Project-URL: issues, https://gitlab.com/scoopgroup-public/scoop-template-engine/issues
 Project-URL: changelog, https://gitlab.com/scoopgroup-public/scoop-template-engine/-/blob/main/CHANGELOG.md
 Keywords: template engine,LaTeX,scientific publishing,journals
```

### Comparing `scoop-template-engine-1.1.0/README.md` & `scoop-template-engine-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/pyproject.toml` & `scoop-template-engine-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/doc/markup.py` & `scoop-template-engine-1.1.1/src/doc/markup.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/doc/scoop-prepare-bibtex-file.pdf` & `scoop-template-engine-1.1.1/src/doc/scoop-prepare-bibtex-file.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 14% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,12 +1,12 @@
 THE SCOOP PREPARE BibTEX FILE TOOL
 ROLAND HERZOG
 
 Abstract. This document describes the Scoop Prepare BibTEX
-File tool (version 1.1.0).
+File tool (version 1.1.1).
 
 Contents
 1. Introduction
 2. Commands
 3. Unconditional Transcriptions
 3.1. Upper-Case Character Protection
 3.2. DATE Field
@@ -15,15 +15,15 @@
 3.5. ORGANIZATION Field
 3.6. SUBTITLE Field
 3.7. @REPORT Entries
 3.8. @COLLECTION Entries
 3.9. Bachelor @THESIS
 3.10. Master @THESIS
 3.11. Ph.D. @THESIS
-3.12. Habilatation @THESIS
+3.12. Habilitation @THESIS
 4. Command Line Options
 4.1. Options Related to Specific Entry Types
 4.2. Options Related to EPRINT fields
 4.3. Options Related to the DOI Field
 4.4. Options Related to the URL Field
 4.5. Options Related to Author Names
 
@@ -289,15 +289,15 @@
 is transcribed into
 @PHDTHESIS{...,
 ... = {...},
 SCHOOL = {Heidelberg University},
 TYPE = {{P}h.{D}. thesis},
 }
 
-3.12. Habilatation @THESIS. spbf convert transcribes entries of type @THESIS
+3.12. Habilitation @THESIS. spbf convert transcribes entries of type @THESIS
 with a TYPE = {Habilitation thesis} field into entries of type @PHDTHESIS
 with a field TYPE = {{H}abilitation thesis}. In this case, it also replaces
 an INSTITUTION field by a SCHOOL field. For instance, an entry
 @THESIS{...,
 ... = {...},
 INSTITUTION = {Heidelberg University},
 TYPE = {Habilitation thesis},
@@ -501,12 +501,28 @@
 EDITOR = {Hoffmann, K.-H.},
 }
 
 14
 
 ROLAND HERZOG
 
+4.5.2. --protectfamilynames. Some .bst files do not correctly handle multipart author and editor family names. This option causes entries of all types
+@...{...,
+AUTHOR = {Hoffmann, Karl-Heinz},
+}
+to be transcribed according to
+@...{...,
+AUTHOR = {{Hoffmann}, K.-H.},
+}
+and entries of all types
+@...{...,
+EDITOR = {Hoffmann, Karl-Heinz},
+}
+to be transcribed according to
+@...{...,
+EDITOR = {{Hoffmann}, K.-H.},
+}
 (R. Herzog) Interdisciplinary Center for Scientific Computing, Heidelberg
 University, 69120 Heidelberg, Germany
 Email address: roland.herzog@iwr.uni-heidelberg.de
```

### Comparing `scoop-template-engine-1.1.0/src/doc/scoop-template-engine.pdf` & `scoop-template-engine-1.1.1/src/doc/scoop-template-engine.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 11% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,12 +1,12 @@
 THE SCOOP TEMPLATE ENGINE
 ROLAND HERZOG
 
 Abstract. This document describes the Scoop Template Engine
-(version 1.1.0).
+(version 1.1.1).
 
 Contents
 Important Note
 1. Installation
 1.1. Installation Without a Virtual Environment
 1.2. Installation Into a Virtual Environment
 1.3. Installation Into a Conda Virtual Environment
@@ -64,32 +64,34 @@
 
 2
 
 ROLAND HERZOG
 
 6.6. Compatibility level testing
 7. Best Practices
-8. Contributing
-9. Known Issues, Limitations
-10. List of Templates
+8. Frontmatter
+9. Contributing
+10. Known Issues, Limitations
+11. List of Templates
 
 33
 33
 35
-35
-36
+37
+37
+38
 
 THE SCOOP TEMPLATE ENGINE
 
 3
 
 The Scoop Template Engine is meant to facilitate the preparation of
 scientific articles written in LATEX, abiding to the formatting standards of
 various scientific journals. It currently supports 377 different journals across
-several disciplines, listed in Section 10. Are you tired of looking up how a
+several disciplines, listed in Section 11. Are you tired of looking up how a
 journal expects you to use its \author, \address and \affil commands?
 Would you rather prefer to format your manuscripts as easily as this?
 ste prepare --template amspreprint
 ste prepare --template sinum
 ste prepare --template crelle
 Then the Scoop Template Engine is for you.
 Important Note
@@ -995,15 +997,15 @@
 USA
 The > indicates YAML folding style, which preserves the content as is but
 converts newlines to spaces. The (optional) - modifier removes any trailing
 newlines that may be following the respective block.
 5. Bibliography
 The Scoop Template Engine supports all three options to handle bibliographies for manuscripts.
 5.1. BibLATEX. Some templates templates process their bibliography using
-BibLATEX, notably amspreprint; see Section 10. For these templates, the
+BibLATEX, notably amspreprint; see Section 11. For these templates, the
 .bib file(s) you specify in the .yaml data file using, e. g.,
 latex:
 bibfiles: manuscript.bib
 will be added directly as bibliographic resource(s) to the generated top-level
 file (such as manuscript-preprint.tex) using \addbibresource. Moreover, a \printbibliography command will be inserted at the end of the
 generated top-level file (such as manuscript-sinum.tex).
 Compile the generated top-level file using, e. g., pdflatex and biber, or more
@@ -1067,15 +1069,15 @@
 
 ROLAND HERZOG
 
 6. Compatibility
 Being able to format a manuscript for a specific journal unfortunately does
 not mean that the LATEX code in your content file (such as content.tex)
 immediately compiles without errors. For instance, the .cls files of some
-journal might load a specific package which may turn out to be incompatible
+journal might load a specific package that may turn out to be incompatible
 with other packages you wish to use. This issue has nothing to do with the
 Scoop Template Engine but rather the design of some journals’ .cls
 files.
 The Scoop Template Engine makes an effort to support the user in
 writing their document in an outlet-independent way. To this end, it offers
 various levels of compatibility support, which can be set using
 latex:
@@ -1108,20 +1110,21 @@
 THE SCOOP TEMPLATE ENGINE
 
 29
 
 6.1. Compatibility level none. In this compability level, no effort is made
 to achieve any degree of compatibility of the journal’s template with the
 user’s LATEX code. This is not recommended and it may very well cause
-the generated top-level file (such as manuscript-sinum.tex) fail to compile.
-For instance, some journals’ .bst files define a \doi command which does
-not handle DOIs with underscores. Moreover, the custom BibTEX file may
-contain \href or \url commands and thus rely on these commands to be
-available, which is not the case for some journal templates unless, e. g., the
-user explicitly loads the hyperref.sty package (through preamble:).
+the generated top-level file (such as manuscript-sinum.tex) fail to compile. For instance, some journals’ .bst files define a \doi command which
+does not handle DOIs with underscores. Moreover, the custom BibTEX file
+(generated behind the scenes by the companion product Scoop Prepare
+BibTEX File spbf) may contain \href or \url commands and thus rely
+on these commands to be available, which is not the case for some journal
+templates unless, e. g., the user explicitly loads the hyperref.sty package
+(through preamble:).
 6.2. Compatibility level minimal. This compatibility level ensures a minimal degree of compatibility between the journal’s template and the user’s
 LATEX code. For illustration purposes, here are some issues and fixes which
 get applied for some templates in compatibility level minimal:
 • Rudimentary \href and \url commands are provided at the beginning of the document. In case those commands already exist they
 will not be overwritten.
 • In case the journal’s .bst file causes the definition of a \doi command
 to be written into the .bbl file which does not handle underscores,
@@ -1157,47 +1160,38 @@
 command such as \usepackage[utf8]{inputenc} through the preamble:
 key of the .yaml data file.
 For illustration purposes, here are some issues and corresponding fixes which
 get applied for some templates in compatibility level packages:
 • The \todo and \comment commands or environments are reset to
 undefined since the changes.sty package defines its own commands
 with the same name.
-• The program.sty package loaded by some of the .cls files makes
-| an active character, which causes tikz.sty to fail loading and
-consequently all packages relying on tikz.sty, including changes.
-sty.8 Therefore, the role of | needs to be reset outside of program
-environments.
 • A part counter needs to be defined for compatibility with cleveref.
-sty.9
-• The \fpage (reference to first page) needs to be redefined when
-hyperref.sty is used.10
+sty.8
 6.4. Compatibility level changes. This compatibility level is meant to
 facilitate the use of the changes.sty package, which can be used to highlight changes in a manuscript. When this compatibility level is enabled,
 LATEX code is automatically inserted into the generated top-level file (such
 as manuscript-sinum.tex) which configures every author of the manuscript
 via an appropriate \definechangesauthor commands, provided that the
 changes.sty actually has been loaded by the user.
 For instance,
 authors:
 - givenname: Lisa M.
 familyname: Simpson
-8https://tex.stackexchange.com/questions/619280/
-9https://tex.stackexchange.com/questions/482167/
-10https://tex.stackexchange.com/questions/371955/
-
-THE SCOOP TEMPLATE ENGINE
-
-31
-
 tag: LMS
 color: blue
 will result in the following command to be inserted into the top-level file’s
 preamble:
 \definechangesauthor[name={Lisa M. Simpson}, color={blue}]{LMS}
 Consequently, commands such as
+8https://tex.stackexchange.com/questions/482167/
+
+THE SCOOP TEMPLATE ENGINE
+
+31
+
 \added[id=LMS]{added text}
 \deleted[id=LMS]{deleted text}
 \replaced[id=LMS]{new text}{old text}
 will then be available. Please refer to the documentation of the changes.sty
 package for more information on how to use these commands.
 Note that selecting the compatibility level changes does not actively load
 the changes.sty package. You will still need to request it, e. g., via
@@ -1215,23 +1209,23 @@
 all markup from the changes.sty package will be suppressed.
 When no color: is specified for an author, the next color out of a palette of
 fallback colors will be used. Color specification is possible within the limits
 of the \definechangesauthor command, which in turn uses xcolor.sty’s
 command \colorlet. Consequently, color specifications as in
 authors:
 - color: blue!80!black
+are valid. Also, you can define custom colors in the preamble, e. g.,
+latex:
+preamble: |\definecolor{myorange}{HTML}{EE7733}
+and use them as an author’s markup color:
 
 32
 
 ROLAND HERZOG
 
-are valid. Also, you can define custom colors in the preamble, e. g.,
-latex:
-preamble: |\definecolor{myorange}{HTML}{EE7733}
-and use them as an author’s markup color:
 authors:
 - color: myorange
 Finally, in order to access, for instance, xcolor.sty’s CornflowerBlue color,
 you could add
 latex:
 prepreamble: |\PassOptionsToPackage{svgnames}{xcolor}
 to your .yaml data file and use
@@ -1250,24 +1244,24 @@
 • proposition
 • remark
 • theorem
 as well as their starred variants assumption*, corollary*, definition*,
 example*, lemma*, proposition*, remark*, theorem*. The policy of implementation is to try and depart as little as possible from the way the .cls file
 of the template provided by the respective publisher handles theorem-like
 environments. This implies that for some templates, all theorem-like environments share a common counter (e. g., Definition 1 may be followed by
-
-THE SCOOP TEMPLATE ENGINE
-
-33
-
 Theorem 2), while for others, they are numbered independently (e. g., Definition 1 is followed by Theorem 1). Moreover, for some templates, theorem-like
 environments are numbered per section (e. g., Theorem 3.1), while for others
 they are not. In some cases, unnumbered theorem-like environments are not
 available, and then the starred environments are mapped to their respective
 numbered counterparts.
+
+THE SCOOP TEMPLATE ENGINE
+
+33
+
 6.6. Compatibility level testing. This compatibility level is meant to be
 used to facilitate the testing of templates. It is of no particular use during
 production. For instance, it turns off the two-column layout in some templates, which otherwise may impede the verification of the list of references.
 7. Best Practices
 (1) It is recommended to place your preamble in a separate file, e. g.,
 manuscript.sty, and specify
 latex:
@@ -1275,47 +1269,47 @@
 in the data file manuscript.yaml. This avoids the need to re-run
 ste prepare whenever you need to make changes to your preamble,
 e. g., add a package.
 (2) When writing the first draft of a manuscript, you may prefer to use
 a template which uses BibLATEX rather than BibTEX, such as the
 amspreprint template. This way, references you add to the .bib
 file (such as manuscript.bib, as specified through the bibfiles:
-setting) will immediately be available and do not require a pass of
-ste prepare.
+setting) will immediately be available for citation.
 By contrast, when you are writing using a BibTEX based template,
 you will either want to use ste prepare with the --nocustombib
-switch11, or else you will have to re-run ste prepare every time
-you \cite a new reference in order to re-create the BibTEX file
-customized to the journal’s .bst file.
+switch9, or else you will have to re-run ste prepare every time you
+\cite a new reference in order to re-create the BibTEX file customized to the journal’s .bst file.
 (3) Some journals’ .cls files load packages that you would also like
 to use. In order to avoid ! LaTeX Error: Option clash for
 package messages, use \PassOptionsToPackage to pass any options
 you wish this package to use through the prepreamble:
-11As described in Section 5, this results in the .bib file (such as manuscript.bib, as
-specified through the bibfiles: setting) to be used directly, instead of the custom .bib
-file generated from it. This may cause issues in case your .bib entries contain features
-not supported by the journal’s .bst file)
+latex:
+prepreamble: |\PassOptionsToPackage{<options>}{<package>}
+and then make sure the package gets loaded through the preamble:
+9As described in Section 5, the --nocustombib switch results in the .bib file (such as
+
+manuscript.bib, as specified through the bibfiles: setting) to be used directly, instead
+of the custom .bib file generated from it. This may cause issues in case your .bib
+entries contain features not supported by the journal’s .bst file, but it may be temporarily
+acceptable.
 
 34
 
 ROLAND HERZOG
 
 latex:
-prepreamble: |\PassOptionsToPackage{<options>}{<package>}
-and then make sure the package gets loaded through the preamble:
-latex:
 preamble: |\usepackage{<package>}
 Since a package gets loaded only once, the \usepackage command
 will be ignored in case the journal’s .cls file already loads the package.
 (4) The available text width can vary widely between journals. When
 formatting a manuscript for various outlets simultaneously, it may
 therefore be necessary to fine-tune breaks in formulas etc. If you wish
 to format your manuscript to look decent with several templates at
 once (such as the amspreprint template and a journal template),
-conditional formatting sometimes comes in handy. Conditional formatting takes decisions based on the .cls file loaded.12 Here is an
+conditional formatting sometimes comes in handy. Conditional formatting takes decisions based on the .cls file loaded.10 Here is an
 example of such a construction for an equation which fits on a single
 line in the cocv template (which uses the document class cocv.cls),
 but requires a line break in templates based on the svjour3.cls
 document class.
 \makeatletter
 \ltx@ifclassloaded{cocv}{%
 \begin{equation}
@@ -1327,26 +1321,26 @@
 ... \\
 ...
 \end{multline}
 }{}
 \makeatother
 You will need to add \usepackage{ltxcmds} to your preamble: in
 order for the command \ltx@ifclassloaded to be available.
-12Of course, conditional formatting can be based on criteria other than the .cls file
+(5) When you are writing a manuscript together with co-authors who
+are not using the Scoop Template Engine themselves, it is up to
+you to generate the top-level .tex and .bib files and share them.
+When you are using a version control system, put the generated toplevel files under version control too. This makes it easy to spot if a
+10Of course, conditional formatting can be based on criteria other than the .cls file
 
 as well.
 
 THE SCOOP TEMPLATE ENGINE
 
 35
 
-(5) When you are writing a manuscript together with co-authors who
-are not using the Scoop Template Engine themselves, it is up to
-you to generate the top-level .tex and .bib files and share them.
-When you are using a version control system, put the generated toplevel files under version control too. This makes it easy to spot if a
 co-author accidentally edits those generated files manually, instead
 of updating the .yaml data file and re-running ste prepare.
 (6) When you find yourself needing to pass lots of arguments to ste,
 such as
 ste prepare --template amspreprint --outdir build \
 --prefix paper --nosuffix
 then you may prefer to configure these settings in the .yaml data file
@@ -1355,71 +1349,140 @@
 template: preprint
 outdir: build
 prefix: paper
 nosuffix: True
 Subsequently, you can simply say
 ste prepare
 and still override the settings from the command line if needed.
-8. Contributing
+8. Frontmatter
+The frontmatter content of a document can be quite complex. This is where
+packages are loaded and custom commands are defined etc. The Scoop
+Template Engine also uses the frontmatter to implement its compatibility
+levels (Section 6), e. g., to ensure its set of theorem-like environments gets
+defined.
+Frontmatter content is included in the following order in the top-level .tex
+file.
+(1) template-specific prepreamble-*.sty
+Some journal templates provide a prepreamble-*.sty file.
+In compatibility level minimal, the prepreamble-*.sty file ensures,
+e. g., that certain packages required by the .cls file get loaded (without requiring the user to do so). Also, certain options are passed to
+packages which may later be loaded.
+In compatibility level packages, the prepreamble-*.sty file is used
+to prevent certain packages from being loaded (by pretending they
+have already been loaded11), due to incompatibility issues.
+11https://tex.stackexchange.com/questions/39415/
+
+36
+
+ROLAND HERZOG
+
+In compatibility level theorems, the prepreamble-*.sty file is used
+to load amsthm.sty or ntheorem.sty.
+(2) user-defined prepreamble:
+The primary purpose of a user-defined prepreamble: is to pass options to a package that may be loaded by the .cls file.
+(3) \documentclass command
+The \documentclass command is issued and the template-specific
+.cls file is executed, which loads and configures further packages.
+(4) template-specific preamble-*.sty
+Some journal templates provide a preamble-*.sty file.
+In compatibility level minimal, the preamble-*.sty file ensures,
+e. g., that fallback \href and \url are defined, which become effective if hyperref.sty is not loaded at \begin{document}.
+In compatibility level packages, the preamble-*.sty file is used to
+undefine or redefine some commands (typically brought in by the
+.cls file) that would cause incompatibilites with a package on the
+list in Section 6.3.
+In compatibility level theorems, the preamble-*.sty file is used to
+load amsthm.sty or ntheorem.sty.
+(5) user-defined preamble:
+This is where the user loads the packages and defines the custom
+commands they require for their manuscript. It is recommended to
+place the preamble’s content in a separate file, e. g., manuscript.sty,
+and specify
+latex:
+preamble: |\usepackage{manuscript}
+
+(6) template-specific postpreamble-*.sty
+Some journal templates provide a postpreamble-*.sty file.
+In compatibility level minimal, the postpreamble-*.sty file ensures,
+e. g., that fallback \href and \url commands are defined, which become effective if hyperref.sty is not loaded at \begin{document}.
+In addition, it redefines the \doi and \doiurl command provided
+by some .cls files so that it handles DOIs with underscores. It
+
+THE SCOOP TEMPLATE ENGINE
+
+37
+
+also defines a dummy \orcidlink command, that is used in case
+orcidlink.sty is not loaded (but does not typeset its contents).
+In compatibility level theorems, the postpreamble-*.sty file is used
+to define a set of theorem-like environments (see Section 6.5), potentially after removing those defined by the .cls file, if necessary.
+There is currently no user-defined postpreamble: setting, which would be a
+natural item (7). You can, however, emulate it by issuing a
+\AtBeginDocument{%
+...
+}
+command as part of the preamble:.
+9. Contributing
 If you are using the Scoop Template Engine, I would like to hear from
 you at roland.herzog@iwr.uni-heidelberg.de. If you would like to help make
 it better, there are various ways in which you can contribute.
 (1) You may file bug reports and feature requests via https://gitlab.
 com/scoopgroup-public/scoop-template-engine/-/issues.
 (2) You may fork the project from https://gitlab.com/scoopgrouppublic/scoop-template-engine, make improvements yourself, and
 send a merge request.
-9. Known Issues, Limitations
-(1) The date: is currently honored only by few templates.
-
-36
-
-ROLAND HERZOG
-
+10. Known Issues, Limitations
+(1) The date: key is currently honored only by few templates.
 (2) Some templates are incompatible with orcidlink.sty’s \orcidlink
-command. In these cases, ORCiDs are not typeset.
+command, and they do not provide their own alternative. In these
+cases, ORCiDs are not typeset.
 (3) There is no support yet to provide a unified choice of packages for the
 typesetting of algorithms, such as algpseudocode and algorithm2e.
 (4) Templates are currently tested with pdflatex on the TEX Live 2022
 distribution only, but should work also on TEX Live 2019 and later.
 There is currently no support for xelatex or other TEX engines.
 Some templates do compile with xelatex, but not all of them.
-(5) Funding and dedication information is currently in the scope of the
-entire manuscript, not on a per-author basis.
+(5) Funding and dedication information is currently interpreted in the
+scope of the entire manuscript, not on a per-author basis.
+
+38
+
+ROLAND HERZOG
+
 (6) There is currently no support for journals operating a double-blind
 peer review process.
 (7) There is currently no support to typeset research highlights, which
 some journals require authors to explicitly list.
 (8) Author biographies and pictures, which some journals offer to include, are not yet supported.
 In case you encounter further problems, please create an issue at https://
 gitlab.com/scoopgroup-public/scoop-template-engine/-/issues.
-10. List of Templates
+11. List of Templates
 The following table lists all 377 templates currently supported. The table is
 sorted by Journal Name.
 • The Template column contains the name of the respective template.
 This is how a template is specified in
 ste prepare --template ...
 or when using the
 control:
 template: ...
 setting in the data file.
 • The BibLaTeX column indicates whether the respective template processes .bib files using BibLATEX or BibTEX.
 * means BibLATEX is used; see Section 5.1 for details.
-
-THE SCOOP TEMPLATE ENGINE
-
-37
-
 - means that BibTEX is used. This implies that ste prepare
 will create a custom BibTEX file (unless the --nocustombib or
 --nobib option is given); see Section 5.2 for details.
 • The Journal Name column contains the full name of the journal the
 respective template is meant for.
 • The Template Location column shows where the respective template resides.
 • The Type column shows the type of template.
 F means that the template is a regular file.
+
+THE SCOOP TEMPLATE ENGINE
+
+39
+
 L means that the template is a symbolic link (i. e., identical to
 some other file-type template).
 
 BibLATEX
 
 *
 *
@@ -1604,15 +1667,15 @@
 L
 L
 L
 L
 
 Type
 
-38
+40
 ROLAND HERZOG
 
 BibLATEX
 
 *
 *
 *
@@ -1800,15 +1863,15 @@
 L
 F
 F
 
 Type
 
 THE SCOOP TEMPLATE ENGINE
-39
+41
 
 BibLATEX
 
 *
 *
 *
 *
@@ -1992,15 +2055,15 @@
 L
 L
 L
 L
 
 Type
 
-40
+42
 ROLAND HERZOG
 
 BibLATEX
 
 *
 *
 *
@@ -2194,15 +2257,15 @@
 L
 L
 L
 F
 F
 
 THE SCOOP TEMPLATE ENGINE
-41
+43
 
 BibLATEX
 
 *
 *
 *
 *
@@ -2388,15 +2451,15 @@
 L
 L
 L
 L
 
 Type
 
-42
+44
 ROLAND HERZOG
 
 BibLATEX
 
 *
 *
 *
@@ -2595,15 +2658,15 @@
 L
 L
 L
 
 Type
 
 THE SCOOP TEMPLATE ENGINE
-43
+45
 
 BibLATEX
 
 *
 *
 *
 *
@@ -2795,15 +2858,15 @@
 L
 L
 F
 L
 F
 L
 
-44
+46
 ROLAND HERZOG
 
 BibLATEX
 
 *
 *
 *
@@ -3000,15 +3063,15 @@
 L
 L
 L
 
 Type
 
 THE SCOOP TEMPLATE ENGINE
-45
+47
 
 BibLATEX
 
 *
 *
 *
 *
@@ -3153,19 +3216,19 @@
 L
 L
 L
 L
 L
 F
 
-46
+48
 ROLAND HERZOG
 
 THE SCOOP TEMPLATE ENGINE
 
-47
+49
 
 (R. Herzog) Interdisciplinary Center for Scientific Computing, Heidelberg
 University, 69120 Heidelberg, Germany
 Email address: roland.herzog@iwr.uni-heidelberg.de
```

### Comparing `scoop-template-engine-1.1.0/src/scoop_template_engine.egg-info/PKG-INFO` & `scoop-template-engine-1.1.1/src/scoop_template_engine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoop-template-engine
-Version: 1.1.0
+Version: 1.1.1
 Summary: Prepare manuscripts in LaTeX
 Author-email: Roland Herzog <roland.herzog@iwr.uni-heidelberg.de>
 Project-URL: homepage, https://gitlab.com/scoopgroup-public/scoop-template-engine
 Project-URL: repository, https://gitlab.com/scoopgroup-public/scoop-template-engine
 Project-URL: issues, https://gitlab.com/scoopgroup-public/scoop-template-engine/issues
 Project-URL: changelog, https://gitlab.com/scoopgroup-public/scoop-template-engine/-/blob/main/CHANGELOG.md
 Keywords: template engine,LaTeX,scientific publishing,journals
```

### Comparing `scoop-template-engine-1.1.0/src/scoop_template_engine.egg-info/SOURCES.txt` & `scoop-template-engine-1.1.1/src/scoop_template_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/spbf/__main__.py` & `scoop-template-engine-1.1.1/src/spbf/__main__.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/__main__.py` & `scoop-template-engine-1.1.1/src/ste/__main__.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-aabmcb.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-aabmcb.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-aaembp.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-aaembp.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-aaemcq.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-aaemcq.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-aamick.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-aamick.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-aanmf6.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-aanmf6.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-aapmcd.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-aapmcd.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-aastgj.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-aastgj.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-abmcb8.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-abmcb8.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-abseba.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-abseba.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-acbcct.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-acbcct.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-accacs.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-accacs.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-achre4.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-achre4.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-achsc5.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-achsc5.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-acncdm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-acncdm.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-acsccc.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-acsccc.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-acscii.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-acscii.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-acsodf.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-acsodf.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-aeacb3.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-aeacb3.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-aeacc4.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-aeacc4.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-aeecco.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-aeecco.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-aelccp.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-aelccp.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-aesccq.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-aesccq.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-aewcaa.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-aewcaa.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-afsthl.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-afsthl.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-aidcbc.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-aidcbc.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-amacgu.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-amacgu.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-amachv.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-amachv.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-amclct.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-amclct.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-amlccd.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-amlccd.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-amlcef.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-amlcef.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-amrcda.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-amrcda.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-anaccx.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-anaccx.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-ancac3.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-ancac3.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-ancham.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-ancham.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-aoiab5.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-aoiab5.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-apaccd.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-apaccd.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-apcach.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-apcach.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-apchd5.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-apchd5.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-aptsfn.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-aptsfn.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-asbcd6.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-asbcd6.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-ascecg.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-ascecg.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-ascefj.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-ascefj.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-bcches.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-bcches.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-bichaw.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-bichaw.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-bomaf6.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-bomaf6.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-cgdefu.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-cgdefu.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-chreay.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-chreay.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-cmatex.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-cmatex.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-crtoec.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-crtoec.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-enfuem.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-enfuem.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-esthag.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-esthag.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-estlcu.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-estlcu.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-iecred.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-iecred.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-inocaj.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-inocaj.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-jaaucr.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-jaaucr.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-jacsat.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-jacsat.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-jafcau.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-jafcau.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-jamsef.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-jamsef.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-jceaax.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-jceaax.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-jceda8.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-jceda8.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-jcisd8.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-jcisd8.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-jctcce.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-jctcce.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-jmcmar.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-jmcmar.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-jnprdf.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-jnprdf.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-joceah.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-joceah.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-jpcafh.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-jpcafh.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-jpcbfk.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-jpcbfk.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-jpccck.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-jpccck.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-jpclcd.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-jpclcd.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-jprobs.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-jprobs.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-langd5.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-langd5.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-mamobx.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-mamobx.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-mpohbp.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-mpohbp.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-nalefd.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-nalefd.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-oprdfk.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-oprdfk.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-orgnd7.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-orgnd7.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/postpreamble-orlef7.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/postpreamble-orlef7.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-aabmcb.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/preamble-jsc.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{preamble-jsc}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -37,10 +37,8 @@
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
 	\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-aaembp.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/svjour3.cls/preamble-jsc.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{preamble-jsc}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -37,10 +37,8 @@
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
 	\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-aaemcq.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/svjour3.cls/preamble-mpc.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{preamble-jsc}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -37,10 +37,8 @@
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
 	\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-aamick.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/svjour3.cls/preamble-opte.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{preamble-jsc}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -37,10 +37,8 @@
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
 	\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-aanmf6.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-aam.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-aapmcd.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-acha.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-aastgj.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-advengsoft.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-abmcb8.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-aim.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-abseba.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-amc.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-acbcct.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-aml.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-accacs.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-apal.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-achre4.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-apm.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-achsc5.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-apnum.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-acncdm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-arcontrol.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-acsccc.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-array.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-acscii.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-bcra.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-acsodf.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-bdr.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-aeacb3.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-bica.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-aeacc4.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-brain.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-aeecco.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-bulsci.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-aelccp.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-cad.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-aesccq.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-cam.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-aewcaa.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-camwa.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-afsthl.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-chaos.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-aidcbc.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-cma.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-amacgu.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-cnsns.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-amachv.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-cocom.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-amclct.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-coisb.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-amlccd.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-cola.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-amlcef.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-comgeo.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-amrcda.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-commatsci.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-anaccx.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-compgeo.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-ancac3.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-compstruc.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-ancham.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-conengprac.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-aoiab5.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-cosrev.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-apaccd.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-cpc.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-apcach.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-csda.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-apchd5.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-csfx.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-aptsfn.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-csl.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-asbcd6.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-dajour.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-ascecg.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-dam.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-ascefj.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-dark.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-bcches.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-difgeo.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-bichaw.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-disc.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-bomaf6.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-disopt.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-cgdefu.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ecocom.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-chreay.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ecolmodel.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-cmatex.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ecosta.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-crtoec.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ejc.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-enfuem.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ejor.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-esthag.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-enganabound.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-estlcu.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-engappai.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-iecred.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-exco.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-inocaj.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-exmath.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-jaaucr.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ffa.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-jacsat.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-finel.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-jafcau.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-fss.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-jamsef.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-geb.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-jceaax.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-geomphys.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-jceda8.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-gmod.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-jcisd8.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-hcc.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-jctcce.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-health.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-jmcmar.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-heliyon.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-jnprdf.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ic.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-joceah.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ijforecast.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-jpcafh.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ime.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-jpcbfk.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-indag.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-jpccck.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ins.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-jpclcd.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ipl.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-jprobs.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jaca.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-langd5.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jalgebra.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-mamobx.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jat.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-mpohbp.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jcmds.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-nalefd.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jco.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-oprdfk.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jcp.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-orgnd7.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jcpx.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/prepreamble-orlef7.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jcss.sty`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-iecred}
+\ProvidesPackage{prepreamble-cma}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,15 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Ensure proper breaking of long URLs.
-\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-aabmcb.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-aabmcb.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-aaembp.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-aaembp.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-aaemcq.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-aaemcq.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-aamick.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-aamick.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-aanmf6.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-aanmf6.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-aapmcd.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-aapmcd.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-aastgj.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-aastgj.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-abmcb8.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-abmcb8.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-abseba.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-abseba.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-acbcct.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-acbcct.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-accacs.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-accacs.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-achre4.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-achre4.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-achsc5.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-achsc5.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-acncdm.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-acncdm.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-acsccc.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-acsccc.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-acscii.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-acscii.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-acsodf.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-acsodf.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-aeacb3.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-aeacb3.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-aeacc4.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-aeacc4.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-aeecco.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-aeecco.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-aelccp.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-aelccp.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-aesccq.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-aesccq.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-aewcaa.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-aewcaa.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-afsthl.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-afsthl.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-aidcbc.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-aidcbc.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-amacgu.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-amacgu.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-amachv.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-amachv.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-amclct.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-amclct.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-amlccd.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-amlccd.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-amlcef.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-amlcef.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-amrcda.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-amrcda.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-anaccx.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-anaccx.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-ancac3.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-ancac3.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-ancham.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-ancham.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-aoiab5.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-aoiab5.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-apaccd.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-apaccd.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-apcach.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-apcach.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-apchd5.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-apchd5.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-aptsfn.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-aptsfn.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-asbcd6.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-asbcd6.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-ascecg.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-ascecg.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-ascefj.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-ascefj.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-bcches.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-bcches.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-bichaw.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-bichaw.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-bomaf6.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-bomaf6.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-cgdefu.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-cgdefu.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-chreay.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-chreay.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-cmatex.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-cmatex.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-crtoec.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-crtoec.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-enfuem.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-enfuem.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-esthag.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-esthag.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-estlcu.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-estlcu.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-iecred.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-iecred.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-inocaj.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-inocaj.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-jaaucr.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-jaaucr.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-jacsat.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-jacsat.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-jafcau.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-jafcau.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-jamsef.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-jamsef.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-jceaax.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-jceaax.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-jceda8.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-jceda8.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-jcisd8.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-jcisd8.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-jctcce.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-jctcce.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-jmcmar.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-jmcmar.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-jnprdf.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-jnprdf.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-joceah.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-joceah.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-jpcafh.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-jpcafh.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-jpcbfk.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-jpcbfk.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-jpccck.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-jpccck.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-jpclcd.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-jpclcd.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-jprobs.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-jprobs.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-langd5.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-langd5.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-mamobx.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-mamobx.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-mpohbp.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-mpohbp.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-nalefd.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-nalefd.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-oprdfk.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-oprdfk.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-orgnd7.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-orgnd7.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ACS/template-orlef7.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/template-orlef7.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/postpreamble-amcomm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/postpreamble-amcomm.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/postpreamble-cpaa.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/postpreamble-cpaa.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/postpreamble-dcds-b.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/postpreamble-dcds-b.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/postpreamble-dcds-s.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/postpreamble-dcds-s.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/postpreamble-dcds.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/postpreamble-dcds.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/postpreamble-eect.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/postpreamble-eect.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/postpreamble-fods.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/postpreamble-fods.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/postpreamble-ipi.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/postpreamble-ipi.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/postpreamble-jcd.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/postpreamble-jcd.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/postpreamble-jdg.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/postpreamble-jdg.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/postpreamble-jgm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/postpreamble-jgm.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/postpreamble-jimo.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/postpreamble-jimo.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/postpreamble-krm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/postpreamble-krm.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/postpreamble-mcrf.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/postpreamble-mcrf.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/postpreamble-mfc.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/postpreamble-mfc.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/postpreamble-naco.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/postpreamble-naco.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/postpreamble-nhm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/postpreamble-nhm.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/template-amcomm.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/template-amcomm.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/template-cpaa.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/template-cpaa.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/template-dcds-b.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/template-dcds-b.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/template-dcds-s.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/template-dcds-s.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/template-dcds.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/template-dcds.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/template-eect.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/template-eect.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/template-fods.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/template-fods.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/template-ipi.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/template-ipi.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/template-jcd.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/template-jcd.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/template-jdg.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/template-jdg.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/template-jgm.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/template-jgm.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/template-jimo.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/template-jimo.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/template-krm.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/template-krm.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/template-mcrf.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/template-mcrf.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/template-mfc.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/template-mfc.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/template-naco.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/template-naco.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AIMS/template-nhm.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AIMS/template-nhm.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AMS/mcom/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AMS/mcom/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AMS/mcom/postpreamble-mcom.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AMS/mcom/postpreamble-mcom.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/AMS/mcom/template-mcom.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/AMS/mcom/template-mcom.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Begell/ijuq/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Begell/ijuq/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Begell/ijuq/postpreamble-ijuq.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Begell/ijuq/postpreamble-ijuq.sty`

 * *Files 0% similar despite different names*

```diff
@@ -75,8 +75,7 @@
 		\fi
 	}{}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
-
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Begell/ijuq/preamble-ijuq.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Begell/ijuq/preamble-ijuq.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Begell/ijuq/template-ijuq.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Begell/ijuq/template-ijuq.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Centre Mersenne/ojmo/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Centre Mersenne/ojmo/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Centre Mersenne/ojmo/postpreamble-ojmo.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Centre Mersenne/ojmo/postpreamble-ojmo.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Centre Mersenne/ojmo/preamble-ojmo.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Centre Mersenne/ojmo/preamble-ojmo.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Centre Mersenne/ojmo/template-ojmo.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Centre Mersenne/ojmo/template-ojmo.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/acvar/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/acvar/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/acvar/postpreamble-acvar.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/acvar/postpreamble-acvar.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/acvar/template-acvar.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/acvar/template-acvar.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/cmam/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/cmam/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/cmam/postpreamble-cmam.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/cmam/postpreamble-cmam.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/cmam/template-cmam.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/cmam/template-cmam.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/crelle/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/crelle/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/crelle/postpreamble-crelle.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/crelle/postpreamble-crelle.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/crelle/preamble-crelle.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/crelle/preamble-crelle.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/crelle/prepreamble-crelle.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/crelle/prepreamble-crelle.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/crelle/template-crelle.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/crelle/template-crelle.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/jip/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/jip/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/jip/postpreamble-jip.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/jip/postpreamble-jip.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/jip/template-jip.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/jip/template-jip.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/jnm/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/jnm/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/jnm/postpreamble-jnm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/jnm/postpreamble-jnm.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/De Gruyter/jnm/template-jnm.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/De Gruyter/jnm/template-jnm.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/EMS/ag/postpreamble-ag.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/EMS/ag/postpreamble-ag.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/EMS/ag/template-ag.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/EMS/ag/template-ag.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/EMS/em/postpreamble-em.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/EMS/em/postpreamble-em.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/EMS/em/template-em.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/EMS/em/template-em.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/EMS/rlm/postpreamble-rlm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/EMS/rlm/postpreamble-rlm.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/EMS/rlm/template-rlm.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/EMS/rlm/template-rlm.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ESAIM/cocv/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ESAIM/cocv/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ESAIM/cocv/postpreamble-cocv.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ESAIM/cocv/postpreamble-cocv.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ESAIM/cocv/template-cocv.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ESAIM/cocv/template-cocv.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ESAIM/m2an/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ESAIM/m2an/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ESAIM/m2an/postpreamble-m2an.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ESAIM/m2an/postpreamble-m2an.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/ESAIM/m2an/template-m2an.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ESAIM/m2an/template-m2an.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-aam.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-aam.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-acha.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-acha.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-advengsoft.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-advengsoft.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-aim.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-aim.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-amc.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-amc.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-aml.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-aml.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-apal.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-apal.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-apm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-apm.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-apnum.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-apnum.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-arcontrol.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-arcontrol.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-array.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-array.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-bcra.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-bcra.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-bdr.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-bdr.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-bica.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-bica.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-brain.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-brain.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-bulsci.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-bulsci.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-cad.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-cad.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-cam.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-cam.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-camwa.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-camwa.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-chaos.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-chaos.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-cma.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-cma.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-cnsns.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-cnsns.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-cocom.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-cocom.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-coisb.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-coisb.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-cola.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-cola.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-comgeo.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-comgeo.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-commatsci.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-commatsci.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-compgeo.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-compgeo.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-compstruc.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-compstruc.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-conengprac.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-conengprac.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-cosrev.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-cosrev.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-cpc.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-cpc.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-csda.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-csda.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-csfx.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-csfx.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-csl.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-csl.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-dajour.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-dajour.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-dam.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-dam.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-dark.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-dark.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-difgeo.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-difgeo.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-disc.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-disc.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-disopt.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-disopt.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ecocom.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ecocom.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ecolmodel.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ecolmodel.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ecosta.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ecosta.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ejc.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ejc.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ejor.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ejor.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-enganabound.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-enganabound.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-engappai.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-engappai.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-exco.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-exco.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-exmath.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-exmath.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ffa.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ffa.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-finel.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-finel.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-fss.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-fss.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-geb.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-geb.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-geomphys.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-geomphys.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-gmod.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-gmod.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-hcc.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-hcc.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-health.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-health.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-heliyon.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-heliyon.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ic.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ic.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ijforecast.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ijforecast.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ime.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ime.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-indag.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-indag.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ins.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ins.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ipl.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-ipl.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jaca.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jaca.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jalgebra.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jalgebra.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jat.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jat.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jcmds.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jcmds.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jco.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jco.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jcp.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jcp.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jcpx.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jcpx.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jcss.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jcss.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jcta.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jcta.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jctb.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jctb.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jde.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jde.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jebo.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jebo.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jeconom.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jeconom.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jedc.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jedc.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jet.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jet.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jfa.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jfa.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jfranklin.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jfranklin.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jlamp.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jlamp.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jmaa.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jmaa.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jmateco.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jmateco.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jnt.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jnt.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jocsci.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jocsci.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jpaa.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jpaa.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jprocont.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jprocont.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jspi.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jspi.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jsymbc.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-jsymbc.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-laa.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-laa.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-matcom.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-matcom.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-matpur.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-matpur.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-mbs.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-mbs.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-mlwa.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-mlwa.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-mss.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-mss.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-na.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-na.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-nahs.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-nahs.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-nanocomnet.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-nanocomnet.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-neunet.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-neunet.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-nlm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-nlm.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-nonrwa.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-nonrwa.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-nppp.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-nppp.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-nuclphysb.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-nuclphysb.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-orl.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-orl.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-padiff.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-padiff.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-patterns.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-patterns.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-physa.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-physa.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-physd.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-physd.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-physleta.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-physleta.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-physletb.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-physletb.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-plrev.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-plrev.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-pmc.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-pmc.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-pr.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-pr.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-red.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-red.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-rico.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-rico.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-rinam.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-rinam.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-sasc.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-sasc.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-spa.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-spa.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-spasta.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-spasta.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-stapro.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-stapro.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-swevo.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-swevo.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-sysconle.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-sysconle.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-tcs.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-tcs.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-topol.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-topol.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-vehcom.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-vehcom.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-wace.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/postpreamble-wace.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-aam.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jcta.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-acha.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jctb.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-advengsoft.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jde.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-aim.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jebo.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-amc.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jeconom.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-aml.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jedc.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-apal.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jet.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-apm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jfa.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-apnum.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jfranklin.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-arcontrol.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jlamp.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-array.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jmaa.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-bcra.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jmateco.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-bdr.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jnt.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-bica.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jocsci.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-brain.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jpaa.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-bulsci.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jprocont.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-cad.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jspi.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-cam.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jsymbc.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-camwa.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-laa.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-chaos.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-matcom.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-cma.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-matpur.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-cnsns.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-mbs.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-cocom.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-mlwa.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-coisb.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-mss.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-cola.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-na.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-comgeo.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-nahs.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-commatsci.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-nanocomnet.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-compgeo.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-neunet.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-compstruc.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-nlm.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-conengprac.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-nonrwa.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-cosrev.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-nppp.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-cpc.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-nuclphysb.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-csda.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-orl.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-csfx.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-padiff.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-csl.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-patterns.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-dajour.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-physa.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-dam.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-physd.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-dark.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-physleta.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-difgeo.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-physletb.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-disc.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-plrev.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-disopt.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-pmc.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ecocom.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-pr.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ecolmodel.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-red.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ecosta.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-rico.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ejc.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-rinam.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ejor.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-sasc.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-enganabound.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-spa.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-engappai.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-spasta.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-exco.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-stapro.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-exmath.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-swevo.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ffa.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-sysconle.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-finel.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-tcs.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-fss.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-topol.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-geb.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-vehcom.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-geomphys.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-wace.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-gmod.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/prepreamble-cma.sty`

 * *Files 1% similar despite different names*

```diff
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-hcc.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/preamble-jota.sty`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{preamble-jota}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+	\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-health.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/jota/preamble-jota.sty`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{preamble-jota}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+	\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-heliyon.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/preamble-bit.sty`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{preamble-bit}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+	\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ic.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/prepreamble-etna.sty`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-etna}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ijforecast.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bit/preamble-bit.sty`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{preamble-bit}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+	\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ime.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/etna/prepreamble-etna.sty`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-etna}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,13 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-indag.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/preamble-ojmo.sty`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{preamble-ojmo}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -24,21 +24,23 @@
 
 % Execute option 'minimal'. 
 \if@scoopcompatibility@minimal
 \fi
 
 % Execute option 'packages'. 
 \if@scoopcompatibility@packages
+% cedram-OJMO.sty defines a '\todo' command, which interferes with
+% a command by the same name defined by changes.sty.
+\let\todo\undefined
 \fi
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
-% Execute option 'theorems'.
+% Execute option 'theorems'. 
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ins.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/preamble-crelle.sty`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{preamble-crelle}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -24,21 +24,23 @@
 
 % Execute option 'minimal'. 
 \if@scoopcompatibility@minimal
 \fi
 
 % Execute option 'packages'. 
 \if@scoopcompatibility@packages
+% degruyter-crelle.cls loads verbatim.sty, which provides a \comment command interfering with
+% a command by the same name defined by changes.sty.
+\let\comment\undefined
 \fi
 
-% Execute option 'changes'.
+% Execute option 'changes'. 
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-ipl.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/preamble-ijcm.sty`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{preamble-ijcm}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -24,21 +24,27 @@
 
 % Execute option 'minimal'. 
 \if@scoopcompatibility@minimal
 \fi
 
 % Execute option 'packages'. 
 \if@scoopcompatibility@packages
+% ws-ijcm.cls defines 'comment' as a theorem-like environment, which interferes with
+% a command by the same name defined by changes.sty.
+\let\comment\undefined
+\let\endcomment\undefined
 \fi
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+	\let\proof\relax
+	\let\endproof\relax
+	\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jaca.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/ijcm/preamble-ijcm.sty`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{preamble-ijcm}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -24,21 +24,27 @@
 
 % Execute option 'minimal'. 
 \if@scoopcompatibility@minimal
 \fi
 
 % Execute option 'packages'. 
 \if@scoopcompatibility@packages
+% ws-ijcm.cls defines 'comment' as a theorem-like environment, which interferes with
+% a command by the same name defined by changes.sty.
+\let\comment\undefined
+\let\endcomment\undefined
 \fi
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+	\let\proof\relax
+	\let\endproof\relax
+	\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jalgebra.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/ifac/preamble-ifac.sty`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{preamble-ifac}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -24,21 +24,26 @@
 
 % Execute option 'minimal'. 
 \if@scoopcompatibility@minimal
 \fi
 
 % Execute option 'packages'. 
 \if@scoopcompatibility@packages
+% Fix to make ifacconf.cls compatible with cleveref.
+% https://tex.stackexchange.com/questions/482167/
+\newcounter{part}
 \fi
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Turn off two-column layout, which impedes reference testing.
+\@TwoColumnfalse
+\@twocolumnfalse
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jat.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/preamble-ifac.sty`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{preamble-ifac}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -24,21 +24,26 @@
 
 % Execute option 'minimal'. 
 \if@scoopcompatibility@minimal
 \fi
 
 % Execute option 'packages'. 
 \if@scoopcompatibility@packages
+% Fix to make ifacconf.cls compatible with cleveref.
+% https://tex.stackexchange.com/questions/482167/
+\newcounter{part}
 \fi
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Turn off two-column layout, which impedes reference testing.
+\@TwoColumnfalse
+\@twocolumnfalse
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jcmds.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-aabmcb.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jco.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-aaembp.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jcp.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-aaemcq.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jcpx.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-aamick.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jcss.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-aanmf6.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jcta.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-aapmcd.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jctb.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-aastgj.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jde.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-abmcb8.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jebo.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-abseba.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jeconom.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-acbcct.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jedc.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-accacs.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jet.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-achre4.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jfa.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-achsc5.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jfranklin.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-acncdm.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jlamp.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-acsccc.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jmaa.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-acscii.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jmateco.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-acsodf.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jnt.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-aeacb3.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jocsci.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-aeacc4.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jpaa.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-aeecco.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jprocont.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-aelccp.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jspi.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-aesccq.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-jsymbc.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-aewcaa.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-laa.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-afsthl.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-matcom.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-aidcbc.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-matpur.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-amacgu.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-mbs.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-amachv.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-mlwa.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-amclct.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-mss.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-amlccd.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-na.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-amlcef.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-nahs.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-amrcda.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-nanocomnet.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-anaccx.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-neunet.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-ancac3.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-nlm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-ancham.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-nonrwa.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-aoiab5.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-nppp.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-apaccd.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-nuclphysb.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-apcach.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-orl.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-apchd5.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-padiff.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-aptsfn.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-patterns.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-asbcd6.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-physa.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-ascecg.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-physd.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-ascefj.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-physleta.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-bcches.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-physletb.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-bichaw.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-plrev.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-bomaf6.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-pmc.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-cgdefu.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-pr.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-chreay.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-red.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-cmatex.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-rico.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-crtoec.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-rinam.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-enfuem.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-sasc.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-esthag.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-spa.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-estlcu.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-spasta.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-iecred.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-stapro.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-inocaj.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-swevo.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-jaaucr.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-sysconle.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-jacsat.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-tcs.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-jafcau.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-topol.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-jamsef.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-vehcom.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-jceaax.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/prepreamble-wace.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-jceda8.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-aam.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-aam.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-acha.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-acha.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-advengsoft.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-advengsoft.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-aim.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-aim.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-amc.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-amc.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-aml.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-aml.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-apal.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-apal.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-apm.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-apm.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-apnum.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-apnum.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-arcontrol.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-arcontrol.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-array.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-array.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-bcra.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-bcra.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-bdr.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-bdr.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-bica.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-bica.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-brain.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-brain.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-bulsci.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-bulsci.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-cad.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-cad.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-cam.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-cam.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-camwa.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-camwa.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-chaos.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-chaos.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-cma.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-cma.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-cnsns.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-cnsns.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-cocom.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-cocom.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-coisb.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-coisb.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-cola.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-cola.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-comgeo.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-comgeo.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-commatsci.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-commatsci.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-compgeo.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-compgeo.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-compstruc.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-compstruc.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-conengprac.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-conengprac.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-cosrev.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-cosrev.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-cpc.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-cpc.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-csda.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-csda.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-csfx.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-csfx.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-csl.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-csl.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-dajour.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-dajour.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-dam.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-dam.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-dark.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-dark.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-difgeo.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-difgeo.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-disc.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-disc.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-disopt.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-disopt.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ecocom.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ecocom.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ecolmodel.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ecolmodel.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ecosta.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ecosta.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ejc.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ejc.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ejor.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ejor.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-enganabound.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-enganabound.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-engappai.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-engappai.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-exco.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-exco.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-exmath.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-exmath.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ffa.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ffa.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-finel.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-finel.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-fss.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-fss.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-geb.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-geb.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-geomphys.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-geomphys.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-gmod.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-gmod.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-hcc.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-hcc.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-health.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-health.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-heliyon.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-heliyon.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ic.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ic.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ijforecast.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ijforecast.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ime.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ime.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-indag.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-indag.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ins.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ins.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ipl.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-ipl.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jaca.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jaca.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jalgebra.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jalgebra.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jat.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jat.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jcmds.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jcmds.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jco.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jco.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jcp.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jcp.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jcpx.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jcpx.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jcss.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jcss.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jcta.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jcta.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jctb.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jctb.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jde.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jde.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jebo.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jebo.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jeconom.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jeconom.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jedc.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jedc.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jet.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jet.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jfa.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jfa.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jfranklin.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jfranklin.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jlamp.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jlamp.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jmaa.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jmaa.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jmateco.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jmateco.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jnt.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jnt.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jocsci.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jocsci.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jpaa.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jpaa.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jprocont.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jprocont.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jspi.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jspi.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jsymbc.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-jsymbc.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-laa.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-laa.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-matcom.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-matcom.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-matpur.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-matpur.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-mbs.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-mbs.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-mlwa.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-mlwa.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-mss.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-mss.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-na.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-na.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-nahs.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-nahs.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-nanocomnet.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-nanocomnet.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-neunet.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-neunet.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-nlm.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-nlm.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-nonrwa.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-nonrwa.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-nppp.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-nppp.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-nuclphysb.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-nuclphysb.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-orl.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-orl.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-padiff.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-padiff.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-patterns.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-patterns.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-physa.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-physa.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-physd.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-physd.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-physleta.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-physleta.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-physletb.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-physletb.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-plrev.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-plrev.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-pmc.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-pmc.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-pr.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-pr.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-red.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-red.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-rico.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-rico.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-rinam.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-rinam.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-sasc.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-sasc.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-spa.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-spa.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-spasta.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-spasta.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-stapro.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-stapro.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-swevo.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-swevo.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-sysconle.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-sysconle.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-tcs.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-tcs.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-topol.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-topol.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-vehcom.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-vehcom.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/elsarticle.cls/template-wace.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/elsarticle.cls/template-wace.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/ifac/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/ifac/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/ifac/postpreamble-ifac.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/ifac/postpreamble-ifac.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/ifac/preamble-ifac.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-jcisd8.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{preamble-ifac}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -24,26 +24,23 @@
 
 % Execute option 'minimal'. 
 \if@scoopcompatibility@minimal
 \fi
 
 % Execute option 'packages'. 
 \if@scoopcompatibility@packages
-% Fix to make ifacconf.cls compatible with cleveref.
-% https://tex.stackexchange.com/questions/482167/
-\newcounter{part}
 \fi
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Turn off two-column layout, which impedes reference testing.
-\@TwoColumnfalse
-\@twocolumnfalse
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Elsevier/ifac/template-ifac.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Elsevier/ifac/template-ifac.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Frontiers/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Frontiers/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Frontiers/postpreamble-fams.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Frontiers/postpreamble-fams.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Frontiers/template-fams.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Frontiers/template-fams.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-bbiici.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-bbiici.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-bioffn.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-bioffn.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-bmbucs.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-bmbucs.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-bpeeae.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-bpeeae.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-cqgrdg.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-cqgrdg.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-dmatb7.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-dmatb7.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-ejphd4.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-ejphd4.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-ejssbg.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-ejssbg.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-erc.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-erc.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-ercl.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-ercl.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-ere.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-ere.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-erenbl.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-erenbl.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-erh.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-erh.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-erisal.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-erisal.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-erlnal.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-erlnal.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-esltac.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-esltac.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-fcsuah.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-fcsuah.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-fpelab.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-fpelab.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-ijemkf.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-ijemkf.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-ip.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-ip.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-isoccm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-isoccm.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-jbrobw.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-jbrobw.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-jcapbp.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-jcapbp.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-jcomel.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-jcomel.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-jionas.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-jionas.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-jmmiez.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-jmmiez.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-jneiez.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-jneiez.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-joopca.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-joopca.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-jpamb5.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-jpamb5.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-jpapbe.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-jpapbe.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-jpapeh.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-jpapeh.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-jpcofp.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-jpcofp.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-jpcogq.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-jpcogq.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-jpeoey.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-jpeoey.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-jpgped.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-jpgped.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-jpmoc4.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-jpmoc4.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-jppokr.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-jppokr.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-jrprea.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-jrprea.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-jsmtc6.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-jsmtc6.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-mafeb2.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-mafeb2.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-mlstck.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-mlstck.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-mmuabd.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-mmuabd.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-mqtaaz.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-mqtaaz.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-mreac3.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-mreac3.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-msmeeu.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-msmeeu.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-mstcep.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-mstcep.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-mtrgau.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-mtrgau.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-nceecn.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-nceecn.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-neaxa4.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-neaxa4.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-nfaub3.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-nfaub3.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-njopfm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-njopfm.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-nnoter.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-nnoter.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-nonle5.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-nonle5.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-nufuau.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-nufuau.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-pberb8.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-pberb8.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-pbhiat.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-pbhiat.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-perndg.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-perndg.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-pheda7.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-pheda7.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-phmba7.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-phmba7.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-phstbo.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-phstbo.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-pmeae3.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-pmeae3.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-ppcfet.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-ppcfet.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-prelcz.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-prelcz.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-psteeu.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-psteeu.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-qstuah.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-qstuah.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-rpphag.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-rpphag.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-smster.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-smster.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-ssteet.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-ssteet.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-stmpcw.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-stmpcw.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/postpreamble-sustef.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/postpreamble-sustef.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-bbiici.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-bbiici.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-bioffn.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-bioffn.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-bmbucs.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-bmbucs.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-bpeeae.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-bpeeae.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-cqgrdg.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-cqgrdg.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-dmatb7.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-dmatb7.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-ejphd4.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-ejphd4.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-ejssbg.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-ejssbg.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-erc.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-erc.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-ercl.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-ercl.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-ere.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-ere.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-erenbl.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-erenbl.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-erh.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-erh.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-erisal.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-erisal.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-erlnal.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-erlnal.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-esltac.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-esltac.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-fcsuah.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-fcsuah.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-fpelab.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-fpelab.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-ijemkf.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-ijemkf.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-ip.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-ip.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-isoccm.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-isoccm.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-jbrobw.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-jbrobw.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-jcapbp.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-jcapbp.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-jcomel.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-jcomel.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-jionas.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-jionas.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-jmmiez.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-jmmiez.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-jneiez.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-jneiez.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-joopca.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-joopca.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-jpamb5.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-jpamb5.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-jpapbe.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-jpapbe.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-jpapeh.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-jpapeh.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-jpcofp.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-jpcofp.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-jpcogq.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-jpcogq.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-jpeoey.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-jpeoey.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-jpgped.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-jpgped.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-jpmoc4.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-jpmoc4.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-jppokr.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-jppokr.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-jrprea.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-jrprea.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-jsmtc6.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-jsmtc6.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-mafeb2.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-mafeb2.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-mlstck.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-mlstck.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-mmuabd.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-mmuabd.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-mqtaaz.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-mqtaaz.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-mreac3.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-mreac3.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-msmeeu.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-msmeeu.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-mstcep.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-mstcep.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-mtrgau.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-mtrgau.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-nceecn.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-nceecn.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-neaxa4.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-neaxa4.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-nfaub3.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-nfaub3.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-njopfm.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-njopfm.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-nnoter.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-nnoter.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-nonle5.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-nonle5.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-nufuau.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-nufuau.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-pberb8.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-pberb8.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-pbhiat.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-pbhiat.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-perndg.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-perndg.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-pheda7.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-pheda7.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-phmba7.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-phmba7.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-phstbo.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-phstbo.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-pmeae3.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-pmeae3.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-ppcfet.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-ppcfet.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-prelcz.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-prelcz.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-psteeu.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-psteeu.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-qstuah.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-qstuah.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-rpphag.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-rpphag.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-smster.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-smster.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-ssteet.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-ssteet.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-stmpcw.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-stmpcw.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IOP/template-sustef.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IOP/template-sustef.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-aa.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-aa.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-acdm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-acdm.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-amspreprint.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-amspreprint.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-bit.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-bit.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-cma.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-cma.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-cmam.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-cmam.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-cocv.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-cocv.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-crelle.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-crelle.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-etna.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-etna.sty`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 % By default, a \newtheorem command is provided through article.cls.
 % It does provide cleveref.sty support but some theorem-like environments are defined previously.
 % Since the default numbering scheme uses shared counters, we have to clear and redefine all theorem-like environments.
+% We therefore use amsthm.sty.
 \if@scoopcompatibility@theorems
 	% Define a command which will clear a single and multiple theorem-like environments.
 	% https://tex.stackexchange.com/questions/459258
 	\def\clear@theorems#1{\@for\next:=#1\do{\expandafter\clear@theorem\expandafter{\next}}}
 	\def\clear@theorem#1{\expandafter\let\csname #1\endcsname\relax\expandafter\let\csname end#1\endcsname\relax}
 	\clear@theorems{corollary,definition,lemma,proposition}
 	\newtheorem{assumption}[theorem]{Assumption}
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-fams.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-fams.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-gamm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-gamm.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-iecred.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-iecred.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-ifac.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-ifac.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-ijcga.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-ijcga.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-ijcm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-ijcm.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-ijuq.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-ijuq.sty`

 * *Files 0% similar despite different names*

```diff
@@ -75,8 +75,7 @@
 		\fi
 	}{}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
-
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-imanum.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-imanum.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-jmiv.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-jmiv.sty`

 * *Files 0% similar despite different names*

```diff
@@ -68,8 +68,7 @@
 		\fi
 	}{}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
-
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-jnsao.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-jnsao.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-jota.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-jota.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-jsc.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-jsc.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-m2an.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-m2an.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-m3as.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-m3as.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-mcom.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-mcom.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-mcrf.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-mcrf.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-mma.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-mma.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-nla.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-nla.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-nme.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-nme.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-ojmo.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-ojmo.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-opt.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-opt.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-pamm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-pamm.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-ppl.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-ppl.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-siims.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-siims.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-siopt.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-siopt.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/postpreamble-zamm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/postpreamble-zamm.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/preamble-acdm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/preamble-acdm.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/preamble-bit.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/preamble-jmiv.sty`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{preamble-bit}
+\ProvidesPackage{preamble-jmiv}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -26,19 +26,19 @@
 \if@scoopcompatibility@minimal
 \fi
 
 % Execute option 'packages'. 
 \if@scoopcompatibility@packages
 \fi
 
-% Execute option 'changes'.
+% Execute option 'changes'. 
 \if@scoopcompatibility@changes
 \fi
 
-% Execute option 'theorems'.
+% Execute option 'theorems'. 
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/preamble-crelle.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/preamble-ijuq.sty`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{preamble-crelle}
+\ProvidesPackage{preamble-ijuq}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -20,24 +20,26 @@
 % Execute option 'none'. 
 \if@scoopcompatibility@none
 \endinput
 \fi
 
 % Execute option 'minimal'. 
 \if@scoopcompatibility@minimal
+% Provide '\href' and '\url' commands in case hyperref.sty is not loaded.
+\AtBeginDocument{%
+	\providecommand{\href}[2]{\detokenize{#2}}
+	\providecommand{\url}[1]{\detokenize{#1}}
+}
 \fi
 
 % Execute option 'packages'. 
 \if@scoopcompatibility@packages
-% degruyter-crelle.cls loads verbatim.sty, which provides a \comment command interfering with
-% a command by the same name defined by changes.sty.
-\let\comment\undefined
 \fi
 
-% Execute option 'changes'. 
+% Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/preamble-ifac.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-jctcce.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{preamble-ifac}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -24,26 +24,23 @@
 
 % Execute option 'minimal'. 
 \if@scoopcompatibility@minimal
 \fi
 
 % Execute option 'packages'. 
 \if@scoopcompatibility@packages
-% Fix to make ifacconf.cls compatible with cleveref.
-% https://tex.stackexchange.com/questions/482167/
-\newcounter{part}
 \fi
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
-% Turn off two-column layout, which impedes reference testing.
-\@TwoColumnfalse
-\@twocolumnfalse
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/preamble-ijcm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-jmcmar.sty`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{preamble-ijcm}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -24,27 +24,23 @@
 
 % Execute option 'minimal'. 
 \if@scoopcompatibility@minimal
 \fi
 
 % Execute option 'packages'. 
 \if@scoopcompatibility@packages
-% ws-ijcm.cls defines 'comment' as a theorem-like environment, which interferes with
-% a command by the same name defined by changes.sty.
-\let\comment\undefined
-\let\endcomment\undefined
 \fi
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\let\proof\relax
-	\let\endproof\relax
-	\RequirePackage{amsthm}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/preamble-ijuq.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bmcart.cls/preamble-acdm.sty`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{preamble-ijuq}
+\ProvidesPackage{preamble-acdm}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -20,29 +20,29 @@
 % Execute option 'none'. 
 \if@scoopcompatibility@none
 \endinput
 \fi
 
 % Execute option 'minimal'. 
 \if@scoopcompatibility@minimal
-% Provide '\href' and '\url' commands in case hyperref.sty is not loaded.
-\AtBeginDocument{%
-	\providecommand{\href}[2]{\detokenize{#2}}
-	\providecommand{\url}[1]{\detokenize{#1}}
-}
 \fi
 
 % Execute option 'packages'. 
+% bmcart.cls is incompatible with newer versions of hyperref.sty and produces a
+% 'TeX capacity exceeded' error when hyperref.sty is loaded. 
 \if@scoopcompatibility@packages
+	\RequirePackage{etoolbox}
+	\patchcmd{\@@printead}{\ead@prefix\saferef}{\ead@prefix}{}{}
 \fi
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
+	\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/preamble-jmiv.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-acom.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/preamble-jota.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-amo.sty`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{preamble-jota}
+\ProvidesPackage{preamble-jmiv}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -26,19 +26,19 @@
 \if@scoopcompatibility@minimal
 \fi
 
 % Execute option 'packages'. 
 \if@scoopcompatibility@packages
 \fi
 
-% Execute option 'changes'.
+% Execute option 'changes'. 
 \if@scoopcompatibility@changes
 \fi
 
-% Execute option 'theorems'.
+% Execute option 'theorems'. 
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/preamble-jsc.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-calcolo.sty`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{preamble-jsc}
+\ProvidesPackage{preamble-jmiv}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -26,19 +26,19 @@
 \if@scoopcompatibility@minimal
 \fi
 
 % Execute option 'packages'. 
 \if@scoopcompatibility@packages
 \fi
 
-% Execute option 'changes'.
+% Execute option 'changes'. 
 \if@scoopcompatibility@changes
 \fi
 
-% Execute option 'theorems'.
+% Execute option 'theorems'. 
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/preamble-ojmo.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-jnprdf.sty`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{preamble-ojmo}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -24,23 +24,23 @@
 
 % Execute option 'minimal'. 
 \if@scoopcompatibility@minimal
 \fi
 
 % Execute option 'packages'. 
 \if@scoopcompatibility@packages
-% cedram-OJMO.sty defines a '\todo' command, which interferes with
-% a command by the same name defined by changes.sty.
-\let\todo\undefined
 \fi
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
-% Execute option 'theorems'. 
+% Execute option 'theorems'.
 \if@scoopcompatibility@theorems
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/prepreamble-cma.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-joceah.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-cma}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{ntheorem}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/prepreamble-crelle.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/prepreamble-crelle.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/prepreamble-etna.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-jpcafh.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-etna}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -37,8 +37,10 @@
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
 \RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/prepreamble-iecred.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-jpcbfk.sty`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 % Ensure proper breaking of long URLs.
 \PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/prepreamble-imanum.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/prepreamble-imanum.sty`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 \if@scoopcompatibility@minimal
 \fi
 
 % Execute option 'packages'. 
 \if@scoopcompatibility@packages
 % Prevent orcidlink.sty from being loaded, which conflicts with the \ORCID
 % command defined in ima-authoring-template.cls. 
-\expandafter\def\csname ver@orcidlink.sty\endcsname{}
 \@namedef{ver@orcidlink.sty}{}
 \fi
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/IntegrationTest/build/prepreamble-jmiv.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/prepreamble-jmiv.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Oxford Academic/imanum/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Oxford Academic/imanum/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Oxford Academic/imanum/postpreamble-imanum.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Oxford Academic/imanum/postpreamble-imanum.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Oxford Academic/imanum/prepreamble-imanum.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Oxford Academic/imanum/prepreamble-imanum.sty`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 \if@scoopcompatibility@minimal
 \fi
 
 % Execute option 'packages'. 
 \if@scoopcompatibility@packages
 % Prevent orcidlink.sty from being loaded, which conflicts with the \ORCID
 % command defined in ima-authoring-template.cls. 
-\expandafter\def\csname ver@orcidlink.sty\endcsname{}
 \@namedef{ver@orcidlink.sty}{}
 \fi
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Oxford Academic/imanum/template-imanum.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Oxford Academic/imanum/template-imanum.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/postpreamble-mms.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/postpreamble-mms.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/postpreamble-siap.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/postpreamble-siap.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/postpreamble-sicomp.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/postpreamble-sicomp.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/postpreamble-sicon.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/postpreamble-sicon.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/postpreamble-sidma.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/postpreamble-sidma.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/postpreamble-sima.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/postpreamble-sima.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/postpreamble-simax.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/postpreamble-simax.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/postpreamble-sinum.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/postpreamble-sinum.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/postpreamble-siopt.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/postpreamble-siopt.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/postpreamble-sirev.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/postpreamble-sirev.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/postpreamble-sisc.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/postpreamble-sisc.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/postpreamble-tvp.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/postpreamble-tvp.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/template-mms.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/template-mms.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/template-siap.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/template-siap.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/template-sicomp.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/template-sicomp.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/template-sicon.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/template-sicon.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/template-sidma.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/template-sidma.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/template-sima.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/template-sima.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/template-simax.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/template-simax.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/template-sinum.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/template-sinum.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/template-siopt.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/template-siopt.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/template-sirev.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/template-sirev.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/template-sisc.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/template-sisc.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAM/template-tvp.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAM/template-tvp.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAMOnline/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAMOnline/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAMOnline/postpreamble-juq.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAMOnline/postpreamble-juq.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAMOnline/postpreamble-siads.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAMOnline/postpreamble-siads.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAMOnline/postpreamble-siaga.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAMOnline/postpreamble-siaga.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAMOnline/postpreamble-sifin.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAMOnline/postpreamble-sifin.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAMOnline/postpreamble-siims.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAMOnline/postpreamble-siims.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAMOnline/postpreamble-simods.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAMOnline/postpreamble-simods.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAMOnline/template-juq.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAMOnline/template-juq.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAMOnline/template-siads.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAMOnline/template-siads.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAMOnline/template-siaga.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAMOnline/template-siaga.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAMOnline/template-sifin.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAMOnline/template-sifin.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAMOnline/template-siims.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAMOnline/template-siims.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/SIAMOnline/template-simods.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/SIAMOnline/template-simods.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bit/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bit/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bit/postpreamble-bit.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bit/postpreamble-bit.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bit/preamble-bit.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-camcos.sty`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{preamble-bit}
+\ProvidesPackage{preamble-jmiv}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -26,19 +26,19 @@
 \if@scoopcompatibility@minimal
 \fi
 
 % Execute option 'packages'. 
 \if@scoopcompatibility@packages
 \fi
 
-% Execute option 'changes'.
+% Execute option 'changes'. 
 \if@scoopcompatibility@changes
 \fi
 
-% Execute option 'theorems'.
+% Execute option 'theorems'. 
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bit/template-bit.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bit/template-bit.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bmcart.cls/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bmcart.cls/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bmcart.cls/postpreamble-acdm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bmcart.cls/postpreamble-acdm.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bmcart.cls/postpreamble-bvp.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bmcart.cls/postpreamble-bvp.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bmcart.cls/postpreamble-jia.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bmcart.cls/postpreamble-jia.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bmcart.cls/postpreamble-jmi.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bmcart.cls/postpreamble-jmi.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bmcart.cls/preamble-acdm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bmcart.cls/preamble-bvp.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bmcart.cls/preamble-bvp.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bmcart.cls/preamble-jia.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bmcart.cls/preamble-jia.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bmcart.cls/preamble-jmi.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bmcart.cls/preamble-jmi.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-jpccck.sty`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{preamble-acdm}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -23,26 +23,24 @@
 \fi
 
 % Execute option 'minimal'. 
 \if@scoopcompatibility@minimal
 \fi
 
 % Execute option 'packages'. 
-% bmcart.cls is incompatible with newer versions of hyperref.sty and produces a
-% 'TeX capacity exceeded' error when hyperref.sty is loaded. 
 \if@scoopcompatibility@packages
-	\RequirePackage{etoolbox}
-	\patchcmd{\@@printead}{\ead@prefix\saferef}{\ead@prefix}{}{}
 \fi
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bmcart.cls/template-acdm.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bmcart.cls/template-acdm.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bmcart.cls/template-bvp.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bmcart.cls/template-bvp.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bmcart.cls/template-jia.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bmcart.cls/template-jia.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/bmcart.cls/template-jmi.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/bmcart.cls/template-jmi.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/jota/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/jota/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/jota/postpreamble-jota.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/jota/postpreamble-jota.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/jota/preamble-jota.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-cm.sty`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{preamble-jota}
+\ProvidesPackage{preamble-jmiv}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -26,19 +26,19 @@
 \if@scoopcompatibility@minimal
 \fi
 
 % Execute option 'packages'. 
 \if@scoopcompatibility@packages
 \fi
 
-% Execute option 'changes'.
+% Execute option 'changes'. 
 \if@scoopcompatibility@changes
 \fi
 
-% Execute option 'theorems'.
+% Execute option 'theorems'. 
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/jota/template-jota.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/jota/template-jota.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-acom.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-acom.sty`

 * *Files 0% similar despite different names*

```diff
@@ -68,8 +68,7 @@
 		\fi
 	}{}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
-
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-amo.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-amo.sty`

 * *Files 0% similar despite different names*

```diff
@@ -68,8 +68,7 @@
 		\fi
 	}{}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
-
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-calcolo.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-calcolo.sty`

 * *Files 0% similar despite different names*

```diff
@@ -68,8 +68,7 @@
 		\fi
 	}{}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
-
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-camcos.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-camcos.sty`

 * *Files 0% similar despite different names*

```diff
@@ -68,8 +68,7 @@
 		\fi
 	}{}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
-
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-cm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-cm.sty`

 * *Files 0% similar despite different names*

```diff
@@ -68,8 +68,7 @@
 		\fi
 	}{}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
-
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-coam.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-coam.sty`

 * *Files 0% similar despite different names*

```diff
@@ -68,8 +68,7 @@
 		\fi
 	}{}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
-
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-coap.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-coap.sty`

 * *Files 0% similar despite different names*

```diff
@@ -68,8 +68,7 @@
 		\fi
 	}{}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
-
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-cvpde.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-cvpde.sty`

 * *Files 0% similar despite different names*

```diff
@@ -68,8 +68,7 @@
 		\fi
 	}{}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
-
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-dcg.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-dcg.sty`

 * *Files 0% similar despite different names*

```diff
@@ -68,8 +68,7 @@
 		\fi
 	}{}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
-
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-focm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-focm.sty`

 * *Files 0% similar despite different names*

```diff
@@ -68,8 +68,7 @@
 		\fi
 	}{}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
-
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-ijot.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-ijot.sty`

 * *Files 0% similar despite different names*

```diff
@@ -68,8 +68,7 @@
 		\fi
 	}{}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
-
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-inge.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-inge.sty`

 * *Files 0% similar despite different names*

```diff
@@ -68,8 +68,7 @@
 		\fi
 	}{}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
-
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-jmiv.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-jmiv.sty`

 * *Files 0% similar despite different names*

```diff
@@ -68,8 +68,7 @@
 		\fi
 	}{}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
-
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-jogo.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-jogo.sty`

 * *Files 0% similar despite different names*

```diff
@@ -68,8 +68,7 @@
 		\fi
 	}{}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
-
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-maana.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-maana.sty`

 * *Files 0% similar despite different names*

```diff
@@ -68,8 +68,7 @@
 		\fi
 	}{}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
-
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-mathbio.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-mathbio.sty`

 * *Files 0% similar despite different names*

```diff
@@ -68,8 +68,7 @@
 		\fi
 	}{}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
-
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-mathprog.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-mathprog.sty`

 * *Files 0% similar despite different names*

```diff
@@ -68,8 +68,7 @@
 		\fi
 	}{}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
-
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-mmor.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-mmor.sty`

 * *Files 0% similar despite different names*

```diff
@@ -68,8 +68,7 @@
 		\fi
 	}{}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
-
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-ms.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-ms.sty`

 * *Files 0% similar despite different names*

```diff
@@ -68,8 +68,7 @@
 		\fi
 	}{}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
-
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-numa.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-numa.sty`

 * *Files 0% similar despite different names*

```diff
@@ -68,8 +68,7 @@
 		\fi
 	}{}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
-
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-numalg.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-numalg.sty`

 * *Files 0% similar despite different names*

```diff
@@ -68,8 +68,7 @@
 		\fi
 	}{}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
-
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-pdea.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-pdea.sty`

 * *Files 0% similar despite different names*

```diff
@@ -68,8 +68,7 @@
 		\fi
 	}{}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
-
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-rm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-rm.sty`

 * *Files 0% similar despite different names*

```diff
@@ -68,8 +68,7 @@
 		\fi
 	}{}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
-
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-svva.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/postpreamble-svva.sty`

 * *Files 0% similar despite different names*

```diff
@@ -68,8 +68,7 @@
 		\fi
 	}{}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
 \fi
-
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-acom.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-coam.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-amo.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-coap.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-calcolo.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-cvpde.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-camcos.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-dcg.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-cm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-focm.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-coam.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-ijot.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-coap.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-inge.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-cvpde.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-jmiv.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-dcg.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-jogo.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-focm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-maana.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-ijot.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-mathbio.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-inge.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-mathprog.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-jmiv.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-mmor.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-jogo.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-ms.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-maana.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-numa.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-mathbio.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-numalg.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-mathprog.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-pdea.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-mmor.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-rm.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-ms.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-svva.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-numa.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-jpclcd.sty`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{preamble-jmiv}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -26,19 +26,21 @@
 \if@scoopcompatibility@minimal
 \fi
 
 % Execute option 'packages'. 
 \if@scoopcompatibility@packages
 \fi
 
-% Execute option 'changes'. 
+% Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
-% Execute option 'theorems'. 
+% Execute option 'theorems'.
 \if@scoopcompatibility@theorems
 \RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-numalg.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-jprobs.sty`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{preamble-jmiv}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -26,19 +26,21 @@
 \if@scoopcompatibility@minimal
 \fi
 
 % Execute option 'packages'. 
 \if@scoopcompatibility@packages
 \fi
 
-% Execute option 'changes'. 
+% Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
-% Execute option 'theorems'. 
+% Execute option 'theorems'.
 \if@scoopcompatibility@theorems
 \RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-pdea.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-langd5.sty`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{preamble-jmiv}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -26,19 +26,21 @@
 \if@scoopcompatibility@minimal
 \fi
 
 % Execute option 'packages'. 
 \if@scoopcompatibility@packages
 \fi
 
-% Execute option 'changes'. 
+% Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
-% Execute option 'theorems'. 
+% Execute option 'theorems'.
 \if@scoopcompatibility@theorems
 \RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-rm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-mamobx.sty`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{preamble-jmiv}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -26,19 +26,21 @@
 \if@scoopcompatibility@minimal
 \fi
 
 % Execute option 'packages'. 
 \if@scoopcompatibility@packages
 \fi
 
-% Execute option 'changes'. 
+% Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
-% Execute option 'theorems'. 
+% Execute option 'theorems'.
 \if@scoopcompatibility@theorems
 \RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/preamble-svva.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-mpohbp.sty`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{preamble-jmiv}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -26,19 +26,21 @@
 \if@scoopcompatibility@minimal
 \fi
 
 % Execute option 'packages'. 
 \if@scoopcompatibility@packages
 \fi
 
-% Execute option 'changes'. 
+% Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
-% Execute option 'theorems'. 
+% Execute option 'theorems'.
 \if@scoopcompatibility@theorems
 \RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-acom.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-acom.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-amo.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-amo.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-calcolo.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-calcolo.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-camcos.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-camcos.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-cm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-cm.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-coam.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-coam.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-coap.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-coap.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-cvpde.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-cvpde.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-dcg.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-dcg.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-focm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-focm.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-ijot.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-ijot.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-inge.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-inge.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-jmiv.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-jmiv.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-jogo.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-jogo.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-maana.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-maana.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-mathbio.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-mathbio.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-mathprog.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-mathprog.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-mmor.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-mmor.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-ms.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-ms.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-numa.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-numa.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-numalg.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-numalg.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-pdea.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-pdea.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-rm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-rm.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-svva.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/prepreamble-svva.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-acom.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-acom.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-amo.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-amo.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-calcolo.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-calcolo.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-camcos.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-camcos.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-cm.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-cm.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-coam.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-coam.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-coap.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-coap.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-cvpde.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-cvpde.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-dcg.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-dcg.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-focm.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-focm.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-ijot.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-ijot.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-inge.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-inge.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-jmiv.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-jmiv.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-jogo.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-jogo.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-maana.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-maana.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-mathbio.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-mathbio.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-mathprog.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-mathprog.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-mmor.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-mmor.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-ms.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-ms.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-numa.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-numa.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-numalg.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-numalg.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-pdea.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-pdea.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-rm.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-rm.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/sn-jnl.cls/template-svva.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/sn-jnl.cls/template-svva.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/svjour3.cls/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/svjour3.cls/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/svjour3.cls/postpreamble-jsc.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/svjour3.cls/postpreamble-jsc.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/svjour3.cls/postpreamble-mpc.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/svjour3.cls/postpreamble-mpc.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/svjour3.cls/postpreamble-opte.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/svjour3.cls/postpreamble-opte.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/svjour3.cls/preamble-jsc.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-nalefd.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{preamble-jsc}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/svjour3.cls/preamble-mpc.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-oprdfk.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{preamble-jsc}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/svjour3.cls/preamble-opte.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-orgnd7.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{preamble-jsc}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -32,13 +32,15 @@
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\RequirePackage{amsthm}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/svjour3.cls/template-jsc.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/svjour3.cls/template-jsc.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/svjour3.cls/template-mpc.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/svjour3.cls/template-mpc.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Springer/svjour3.cls/template-opte.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Springer/svjour3.cls/template-opte.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/TaylorAndFrancis/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/TaylorAndFrancis/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/TaylorAndFrancis/postpreamble-apa.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/TaylorAndFrancis/postpreamble-apa.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/TaylorAndFrancis/postpreamble-eno.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/TaylorAndFrancis/postpreamble-eno.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/TaylorAndFrancis/postpreamble-oms.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/TaylorAndFrancis/postpreamble-oms.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/TaylorAndFrancis/postpreamble-opt.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/TaylorAndFrancis/postpreamble-opt.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/TaylorAndFrancis/template-apa.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/TaylorAndFrancis/template-apa.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/TaylorAndFrancis/template-eno.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/TaylorAndFrancis/template-eno.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/TaylorAndFrancis/template-oms.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/TaylorAndFrancis/template-oms.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/TaylorAndFrancis/template-opt.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/TaylorAndFrancis/template-opt.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/gamm/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/gamm/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/gamm/postpreamble-gamm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/gamm/postpreamble-gamm.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/gamm/template-gamm.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/gamm/template-gamm.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/mma/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/mma/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/mma/postpreamble-mma.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/mma/postpreamble-mma.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/mma/template-mma.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/mma/template-mma.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/nla/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/nla/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/nla/postpreamble-nla.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/nla/postpreamble-nla.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/nla/template-nla.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/nla/template-nla.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/nme/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/nme/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/nme/postpreamble-nme.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/nme/postpreamble-nme.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/nme/template-nme.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/nme/template-nme.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/pamm/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/pamm/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/pamm/postpreamble-pamm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/pamm/postpreamble-pamm.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/pamm/template-pamm.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/pamm/template-pamm.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/zamm/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/zamm/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/zamm/postpreamble-zamm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/zamm/postpreamble-zamm.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/Wiley/zamm/template-zamm.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/Wiley/zamm/template-zamm.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/aa/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/aa/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/aa/postpreamble-aa.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/aa/postpreamble-aa.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/aa/template-aa.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/aa/template-aa.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/ijcga/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/ijcga/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/ijcga/postpreamble-ijcga.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/ijcga/postpreamble-ijcga.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/ijcga/template-ijcga.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/ijcga/template-ijcga.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/ijcm/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/ijcm/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/ijcm/postpreamble-ijcm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/ijcm/postpreamble-ijcm.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/ijcm/preamble-ijcm.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/ACS/prepreamble-orlef7.sty`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{preamble-ijcm}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -24,27 +24,23 @@
 
 % Execute option 'minimal'. 
 \if@scoopcompatibility@minimal
 \fi
 
 % Execute option 'packages'. 
 \if@scoopcompatibility@packages
-% ws-ijcm.cls defines 'comment' as a theorem-like environment, which interferes with
-% a command by the same name defined by changes.sty.
-\let\comment\undefined
-\let\endcomment\undefined
 \fi
 
 % Execute option 'changes'.
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
-	\let\proof\relax
-	\let\endproof\relax
-	\RequirePackage{amsthm}
+\RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/ijcm/template-ijcm.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/ijcm/template-ijcm.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/m3as/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/m3as/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/m3as/postpreamble-m3as.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/m3as/postpreamble-m3as.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/m3as/template-m3as.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/m3as/template-m3as.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/ppl/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/ppl/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/ppl/postpreamble-ppl.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/ppl/postpreamble-ppl.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/ppl/template-ppl.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/ppl/template-ppl.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/World Scientific/ppl/ws-ppl.bst.patch` & `scoop-template-engine-1.1.1/src/ste/manuscripts/World Scientific/ppl/ws-ppl.bst.patch`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/etna/etna.cls.patch` & `scoop-template-engine-1.1.1/src/ste/manuscripts/etna/etna.cls.patch`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/etna/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/etna/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/etna/postpreamble-etna.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/etna/postpreamble-etna.sty`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 \if@scoopcompatibility@changes
 \fi
 
 % Execute option 'theorems'.
 % By default, a \newtheorem command is provided through article.cls.
 % It does provide cleveref.sty support but some theorem-like environments are defined previously.
 % Since the default numbering scheme uses shared counters, we have to clear and redefine all theorem-like environments.
+% We therefore use amsthm.sty.
 \if@scoopcompatibility@theorems
 	% Define a command which will clear a single and multiple theorem-like environments.
 	% https://tex.stackexchange.com/questions/459258
 	\def\clear@theorems#1{\@for\next:=#1\do{\expandafter\clear@theorem\expandafter{\next}}}
 	\def\clear@theorem#1{\expandafter\let\csname #1\endcsname\relax\expandafter\let\csname end#1\endcsname\relax}
 	\clear@theorems{corollary,definition,lemma,proposition}
 	\newtheorem{assumption}[theorem]{Assumption}
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/etna/prepreamble-etna.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/IntegrationTest/build/prepreamble-iecred.sty`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-\ProvidesPackage{prepreamble-etna}
+\ProvidesPackage{prepreamble-iecred}
 
 % Declare all options.
 \newif\if@scoopcompatibility@none
 \newif\if@scoopcompatibility@minimal
 \newif\if@scoopcompatibility@packages
 \newif\if@scoopcompatibility@changes
 \newif\if@scoopcompatibility@theorems
@@ -37,8 +37,10 @@
 % Execute option 'theorems'.
 \if@scoopcompatibility@theorems
 \RequirePackage{amsthm}
 \fi
 
 % Execute option 'testing'. 
 \if@scoopcompatibility@testing
+% Ensure proper breaking of long URLs.
+\PassOptionsToPackage{hyphens}{url}
 \fi
```

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/etna/template-etna.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/etna/template-etna.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/jnsao/init.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/jnsao/init.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/jnsao/postpreamble-jnsao.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/jnsao/postpreamble-jnsao.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/jnsao/template-jnsao.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/jnsao/template-jnsao.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/manuscripts.py` & `scoop-template-engine-1.1.1/src/ste/manuscripts/manuscripts.py`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/scoop/postpreamble-amspreprint.sty` & `scoop-template-engine-1.1.1/src/ste/manuscripts/scoop/postpreamble-amspreprint.sty`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/scoop/template-amspreprint.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/scoop/template-amspreprint.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/manuscripts/scoop/template-bibgenerator.tex` & `scoop-template-engine-1.1.1/src/ste/manuscripts/scoop/template-bibgenerator.tex`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/schemes/manuscript/manuscript.yaml` & `scoop-template-engine-1.1.1/src/ste/schemes/manuscript/manuscript.yaml`

 * *Files identical despite different names*

### Comparing `scoop-template-engine-1.1.0/src/ste/utilities/utilities.py` & `scoop-template-engine-1.1.1/src/ste/utilities/utilities.py`

 * *Files identical despite different names*

