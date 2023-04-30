# Comparing `tmp/gallery_dl-1.8.7.tar.gz` & `tmp/gallery_dl-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gallery_dl-1.8.7.tar", last modified: Fri Jun 28 18:54:23 2019, max compression
+gzip compressed data, was "dist/gallery_dl-1.9.0.tar", last modified: Fri Jul 19 19:42:17 2019, max compression
```

## Comparing `gallery_dl-1.8.7.tar` & `gallery_dl-1.9.0.tar`

### file list

```diff
@@ -1,161 +1,163 @@
-drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2019-06-28 18:54:23.000000 gallery_dl-1.8.7/
--rw-r--r--   0 mike      (1000) mike      (1000)    10339 2019-06-28 18:54:23.000000 gallery_dl-1.8.7/PKG-INFO
--rw-r--r--   0 mike      (1000) mike      (1000)     7146 2019-06-28 18:54:16.000000 gallery_dl-1.8.7/README.rst
--rw-r--r--   0 mike      (1000) mike      (1000)     4836 2019-06-28 18:54:10.000000 gallery_dl-1.8.7/gallery-dl.1
--rw-r--r--   0 mike      (1000) mike      (1000)     1009 2019-06-28 18:54:11.000000 gallery_dl-1.8.7/gallery-dl.bash_completion
--rw-r--r--   0 mike      (1000) mike      (1000)    39173 2019-06-28 18:54:10.000000 gallery_dl-1.8.7/gallery-dl.conf.5
-drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2019-06-28 18:54:23.000000 gallery_dl-1.8.7/gallery_dl/
--rw-r--r--   0 mike      (1000) mike      (1000)     8529 2019-06-12 16:38:11.000000 gallery_dl-1.8.7/gallery_dl/__init__.py
--rw-r--r--   0 mike      (1000) mike      (1000)      540 2019-02-19 14:28:59.000000 gallery_dl-1.8.7/gallery_dl/__main__.py
--rw-r--r--   0 mike      (1000) mike      (1000)    12048 2019-06-03 18:07:03.000000 gallery_dl-1.8.7/gallery_dl/aes.py
--rw-r--r--   0 mike      (1000) mike      (1000)     5744 2019-06-20 13:36:46.000000 gallery_dl-1.8.7/gallery_dl/cache.py
--rw-r--r--   0 mike      (1000) mike      (1000)     5827 2019-06-03 18:07:03.000000 gallery_dl-1.8.7/gallery_dl/cloudflare.py
--rw-r--r--   0 mike      (1000) mike      (1000)     3915 2019-06-10 09:57:58.000000 gallery_dl-1.8.7/gallery_dl/config.py
-drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2019-06-28 18:54:23.000000 gallery_dl-1.8.7/gallery_dl/downloader/
--rw-r--r--   0 mike      (1000) mike      (1000)      938 2019-06-27 16:30:40.000000 gallery_dl-1.8.7/gallery_dl/downloader/__init__.py
--rw-r--r--   0 mike      (1000) mike      (1000)     5455 2019-06-27 16:30:40.000000 gallery_dl-1.8.7/gallery_dl/downloader/common.py
--rw-r--r--   0 mike      (1000) mike      (1000)     4022 2019-06-27 16:30:40.000000 gallery_dl-1.8.7/gallery_dl/downloader/http.py
--rw-r--r--   0 mike      (1000) mike      (1000)      866 2019-06-27 16:30:40.000000 gallery_dl-1.8.7/gallery_dl/downloader/text.py
--rw-r--r--   0 mike      (1000) mike      (1000)     2689 2019-06-27 16:30:40.000000 gallery_dl-1.8.7/gallery_dl/downloader/ytdl.py
--rw-r--r--   0 mike      (1000) mike      (1000)     1898 2019-02-06 06:57:23.000000 gallery_dl-1.8.7/gallery_dl/exception.py
-drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2019-06-28 18:54:23.000000 gallery_dl-1.8.7/gallery_dl/extractor/
--rw-r--r--   0 mike      (1000) mike      (1000)     3255 2019-06-03 18:07:03.000000 gallery_dl-1.8.7/gallery_dl/extractor/2chan.py
--rw-r--r--   0 mike      (1000) mike      (1000)     6934 2019-06-03 18:07:03.000000 gallery_dl-1.8.7/gallery_dl/extractor/35photo.py
--rw-r--r--   0 mike      (1000) mike      (1000)     3072 2019-06-03 18:07:03.000000 gallery_dl-1.8.7/gallery_dl/extractor/3dbooru.py
--rw-r--r--   0 mike      (1000) mike      (1000)     1357 2019-06-03 18:07:03.000000 gallery_dl-1.8.7/gallery_dl/extractor/4chan.py
--rw-r--r--   0 mike      (1000) mike      (1000)     8177 2019-06-03 18:07:03.000000 gallery_dl-1.8.7/gallery_dl/extractor/500px.py
--rw-r--r--   0 mike      (1000) mike      (1000)     1087 2019-06-03 18:07:03.000000 gallery_dl-1.8.7/gallery_dl/extractor/8chan.py
--rw-r--r--   0 mike      (1000) mike      (1000)     4604 2019-06-14 10:19:24.000000 gallery_dl-1.8.7/gallery_dl/extractor/8muses.py
--rw-r--r--   0 mike      (1000) mike      (1000)     3772 2019-06-27 16:30:40.000000 gallery_dl-1.8.7/gallery_dl/extractor/__init__.py
--rw-r--r--   0 mike      (1000) mike      (1000)    13280 2019-06-03 18:07:03.000000 gallery_dl-1.8.7/gallery_dl/extractor/artstation.py
--rw-r--r--   0 mike      (1000) mike      (1000)     6219 2019-06-03 18:07:03.000000 gallery_dl-1.8.7/gallery_dl/extractor/behance.py
--rw-r--r--   0 mike      (1000) mike      (1000)     3912 2019-06-03 18:07:03.000000 gallery_dl-1.8.7/gallery_dl/extractor/bobx.py
--rw-r--r--   0 mike      (1000) mike      (1000)     7965 2019-06-03 18:07:03.000000 gallery_dl-1.8.7/gallery_dl/extractor/booru.py
--rw-r--r--   0 mike      (1000) mike      (1000)     2090 2019-06-03 18:07:03.000000 gallery_dl-1.8.7/gallery_dl/extractor/chan.py
--rw-r--r--   0 mike      (1000) mike      (1000)    13766 2019-06-24 16:24:19.000000 gallery_dl-1.8.7/gallery_dl/extractor/common.py
--rw-r--r--   0 mike      (1000) mike      (1000)     3112 2019-06-03 18:07:03.000000 gallery_dl-1.8.7/gallery_dl/extractor/danbooru.py
--rw-r--r--   0 mike      (1000) mike      (1000)    37172 2019-06-27 16:30:40.000000 gallery_dl-1.8.7/gallery_dl/extractor/deviantart.py
--rw-r--r--   0 mike      (1000) mike      (1000)     2166 2019-06-03 18:07:03.000000 gallery_dl-1.8.7/gallery_dl/extractor/directlink.py
--rw-r--r--   0 mike      (1000) mike      (1000)     5033 2019-06-03 18:07:03.000000 gallery_dl-1.8.7/gallery_dl/extractor/dynastyscans.py
--rw-r--r--   0 mike      (1000) mike      (1000)     2510 2019-06-03 18:07:03.000000 gallery_dl-1.8.7/gallery_dl/extractor/e621.py
--rw-r--r--   0 mike      (1000) mike      (1000)    13817 2019-06-03 18:07:03.000000 gallery_dl-1.8.7/gallery_dl/extractor/exhentai.py
--rw-r--r--   0 mike      (1000) mike      (1000)     3889 2019-06-03 18:07:03.000000 gallery_dl-1.8.7/gallery_dl/extractor/fallenangels.py
--rw-r--r--   0 mike      (1000) mike      (1000)    18538 2019-06-03 18:07:03.000000 gallery_dl-1.8.7/gallery_dl/extractor/flickr.py
--rw-r--r--   0 mike      (1000) mike      (1000)     5395 2019-06-03 18:07:03.000000 gallery_dl-1.8.7/gallery_dl/extractor/foolfuuka.py
--rw-r--r--   0 mike      (1000) mike      (1000)     9025 2019-06-03 18:07:03.000000 gallery_dl-1.8.7/gallery_dl/extractor/foolslide.py
--rw-r--r--   0 mike      (1000) mike      (1000)     4720 2019-06-03 18:07:03.000000 gallery_dl-1.8.7/gallery_dl/extractor/gelbooru.py
--rw-r--r--   0 mike      (1000) mike      (1000)     2933 2019-06-03 18:07:03.000000 gallery_dl-1.8.7/gallery_dl/extractor/gfycat.py
--rw-r--r--   0 mike      (1000) mike      (1000)     3843 2019-06-03 18:07:03.000000 gallery_dl-1.8.7/gallery_dl/extractor/hbrowse.py
--rw-r--r--   0 mike      (1000) mike      (1000)     3800 2019-06-03 18:07:03.000000 gallery_dl-1.8.7/gallery_dl/extractor/hentai2read.py
--rw-r--r--   0 mike      (1000) mike      (1000)     3200 2019-06-27 16:30:40.000000 gallery_dl-1.8.7/gallery_dl/extractor/hentaicafe.py
--rw-r--r--   0 mike      (1000) mike      (1000)     9967 2019-06-27 16:30:40.000000 gallery_dl-1.8.7/gallery_dl/extractor/hentaifoundry.py
--rw-r--r--   0 mike      (1000) mike      (1000)     4417 2019-06-03 18:07:03.000000 gallery_dl-1.8.7/gallery_dl/extractor/hentaifox.py
--rw-r--r--   0 mike      (1000) mike      (1000)     3843 2019-06-03 18:07:03.000000 gallery_dl-1.8.7/gallery_dl/extractor/hentaihere.py
--rw-r--r--   0 mike      (1000) mike      (1000)     3695 2019-06-03 18:07:03.000000 gallery_dl-1.8.7/gallery_dl/extractor/hentainexus.py
--rw-r--r--   0 mike      (1000) mike      (1000)     3956 2019-06-27 18:24:42.000000 gallery_dl-1.8.7/gallery_dl/extractor/hitomi.py
--rw-r--r--   0 mike      (1000) mike      (1000)     2527 2019-06-03 18:07:03.000000 gallery_dl-1.8.7/gallery_dl/extractor/hypnohub.py
--rw-r--r--   0 mike      (1000) mike      (1000)     2148 2019-06-03 18:07:03.000000 gallery_dl-1.8.7/gallery_dl/extractor/idolcomplex.py
--rw-r--r--   0 mike      (1000) mike      (1000)     4771 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/imagebam.py
--rw-r--r--   0 mike      (1000) mike      (1000)     7400 2019-06-27 16:30:40.000000 gallery_dl-1.8.7/gallery_dl/extractor/imagefap.py
--rw-r--r--   0 mike      (1000) mike      (1000)     9146 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/imagehosts.py
--rw-r--r--   0 mike      (1000) mike      (1000)     4561 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/imgbox.py
--rw-r--r--   0 mike      (1000) mike      (1000)     2292 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/imgth.py
--rw-r--r--   0 mike      (1000) mike      (1000)     6668 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/imgur.py
--rw-r--r--   0 mike      (1000) mike      (1000)     9923 2019-06-27 16:30:40.000000 gallery_dl-1.8.7/gallery_dl/extractor/instagram.py
--rw-r--r--   0 mike      (1000) mike      (1000)     5315 2019-06-27 16:30:40.000000 gallery_dl-1.8.7/gallery_dl/extractor/keenspot.py
--rw-r--r--   0 mike      (1000) mike      (1000)     2852 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/khinsider.py
--rw-r--r--   0 mike      (1000) mike      (1000)     8187 2019-06-28 18:40:54.000000 gallery_dl-1.8.7/gallery_dl/extractor/kissmanga.py
--rw-r--r--   0 mike      (1000) mike      (1000)     4134 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/komikcast.py
--rw-r--r--   0 mike      (1000) mike      (1000)     3035 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/konachan.py
--rw-r--r--   0 mike      (1000) mike      (1000)     5318 2019-06-06 08:45:38.000000 gallery_dl-1.8.7/gallery_dl/extractor/livedoor.py
--rw-r--r--   0 mike      (1000) mike      (1000)     8191 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/luscious.py
--rw-r--r--   0 mike      (1000) mike      (1000)     6336 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/mangadex.py
--rw-r--r--   0 mike      (1000) mike      (1000)     2292 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/mangafox.py
--rw-r--r--   0 mike      (1000) mike      (1000)     5160 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/mangahere.py
--rw-r--r--   0 mike      (1000) mike      (1000)     1377 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/mangapanda.py
--rw-r--r--   0 mike      (1000) mike      (1000)     5358 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/mangapark.py
--rw-r--r--   0 mike      (1000) mike      (1000)     4673 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/mangareader.py
--rw-r--r--   0 mike      (1000) mike      (1000)     1995 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/mangastream.py
--rw-r--r--   0 mike      (1000) mike      (1000)     5902 2019-06-27 16:30:40.000000 gallery_dl-1.8.7/gallery_dl/extractor/mangoxo.py
--rw-r--r--   0 mike      (1000) mike      (1000)     6696 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/mastodon.py
--rw-r--r--   0 mike      (1000) mike      (1000)     1800 2019-03-14 21:16:42.000000 gallery_dl-1.8.7/gallery_dl/extractor/message.py
--rw-r--r--   0 mike      (1000) mike      (1000)     3445 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/myportfolio.py
--rw-r--r--   0 mike      (1000) mike      (1000)     5628 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/newgrounds.py
--rw-r--r--   0 mike      (1000) mike      (1000)     1661 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/ngomik.py
--rw-r--r--   0 mike      (1000) mike      (1000)     4505 2019-06-17 18:01:25.000000 gallery_dl-1.8.7/gallery_dl/extractor/nhentai.py
--rw-r--r--   0 mike      (1000) mike      (1000)     7421 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/nijie.py
--rw-r--r--   0 mike      (1000) mike      (1000)     2254 2019-06-27 16:30:40.000000 gallery_dl-1.8.7/gallery_dl/extractor/nsfwalbum.py
--rw-r--r--   0 mike      (1000) mike      (1000)    11257 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/oauth.py
--rw-r--r--   0 mike      (1000) mike      (1000)     4142 2019-06-05 09:39:49.000000 gallery_dl-1.8.7/gallery_dl/extractor/paheal.py
--rw-r--r--   0 mike      (1000) mike      (1000)     6219 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/patreon.py
--rw-r--r--   0 mike      (1000) mike      (1000)     6725 2019-06-10 12:58:39.000000 gallery_dl-1.8.7/gallery_dl/extractor/photobucket.py
--rw-r--r--   0 mike      (1000) mike      (1000)     3917 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/piczel.py
--rw-r--r--   0 mike      (1000) mike      (1000)     8905 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/pinterest.py
--rw-r--r--   0 mike      (1000) mike      (1000)    18239 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/pixiv.py
--rw-r--r--   0 mike      (1000) mike      (1000)     6597 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/pixnet.py
--rw-r--r--   0 mike      (1000) mike      (1000)     4123 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/plurk.py
--rw-r--r--   0 mike      (1000) mike      (1000)     5415 2019-06-07 14:27:33.000000 gallery_dl-1.8.7/gallery_dl/extractor/pornhub.py
--rw-r--r--   0 mike      (1000) mike      (1000)     3795 2019-06-27 16:30:40.000000 gallery_dl-1.8.7/gallery_dl/extractor/pururin.py
--rw-r--r--   0 mike      (1000) mike      (1000)    11643 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/reactor.py
--rw-r--r--   0 mike      (1000) mike      (1000)     3598 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/readcomiconline.py
--rw-r--r--   0 mike      (1000) mike      (1000)     1672 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/recursive.py
--rw-r--r--   0 mike      (1000) mike      (1000)    12046 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/reddit.py
--rw-r--r--   0 mike      (1000) mike      (1000)     2385 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/rule34.py
--rw-r--r--   0 mike      (1000) mike      (1000)     2453 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/safebooru.py
--rw-r--r--   0 mike      (1000) mike      (1000)    10524 2019-06-28 15:14:18.000000 gallery_dl-1.8.7/gallery_dl/extractor/sankaku.py
--rw-r--r--   0 mike      (1000) mike      (1000)     4145 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/sankakucomplex.py
--rw-r--r--   0 mike      (1000) mike      (1000)     7123 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/seiga.py
--rw-r--r--   0 mike      (1000) mike      (1000)     2500 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/senmanga.py
--rw-r--r--   0 mike      (1000) mike      (1000)     6471 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/sexcom.py
--rw-r--r--   0 mike      (1000) mike      (1000)     4513 2019-06-05 09:32:47.000000 gallery_dl-1.8.7/gallery_dl/extractor/shopify.py
--rw-r--r--   0 mike      (1000) mike      (1000)     7446 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/simplyhentai.py
--rw-r--r--   0 mike      (1000) mike      (1000)     4550 2019-06-14 16:40:11.000000 gallery_dl-1.8.7/gallery_dl/extractor/slickpic.py
--rw-r--r--   0 mike      (1000) mike      (1000)     3329 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/slideshare.py
--rw-r--r--   0 mike      (1000) mike      (1000)    10598 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/smugmug.py
--rw-r--r--   0 mike      (1000) mike      (1000)     2488 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/test.py
--rw-r--r--   0 mike      (1000) mike      (1000)    11746 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/tsumino.py
--rw-r--r--   0 mike      (1000) mike      (1000)    14402 2019-06-04 11:56:02.000000 gallery_dl-1.8.7/gallery_dl/extractor/tumblr.py
--rw-r--r--   0 mike      (1000) mike      (1000)     7269 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/twitter.py
--rw-r--r--   0 mike      (1000) mike      (1000)     3368 2019-06-27 16:30:40.000000 gallery_dl-1.8.7/gallery_dl/extractor/vanillarock.py
--rw-r--r--   0 mike      (1000) mike      (1000)     5173 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/wallhaven.py
--rw-r--r--   0 mike      (1000) mike      (1000)     4054 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/warosu.py
--rw-r--r--   0 mike      (1000) mike      (1000)     4641 2019-06-22 18:50:48.000000 gallery_dl-1.8.7/gallery_dl/extractor/weibo.py
--rw-r--r--   0 mike      (1000) mike      (1000)     4395 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/wikiart.py
--rw-r--r--   0 mike      (1000) mike      (1000)     5927 2019-06-06 20:36:49.000000 gallery_dl-1.8.7/gallery_dl/extractor/xhamster.py
--rw-r--r--   0 mike      (1000) mike      (1000)     5009 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/xvideos.py
--rw-r--r--   0 mike      (1000) mike      (1000)     2413 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/yandere.py
--rw-r--r--   0 mike      (1000) mike      (1000)     4021 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/yaplog.py
--rw-r--r--   0 mike      (1000) mike      (1000)     4549 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/extractor/yuki.py
--rw-r--r--   0 mike      (1000) mike      (1000)    16850 2019-06-27 16:30:40.000000 gallery_dl-1.8.7/gallery_dl/job.py
--rw-r--r--   0 mike      (1000) mike      (1000)     4218 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/oauth.py
--rw-r--r--   0 mike      (1000) mike      (1000)    10590 2019-06-27 16:30:40.000000 gallery_dl-1.8.7/gallery_dl/option.py
--rw-r--r--   0 mike      (1000) mike      (1000)     6509 2019-06-27 16:30:40.000000 gallery_dl-1.8.7/gallery_dl/output.py
-drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2019-06-28 18:54:23.000000 gallery_dl-1.8.7/gallery_dl/postprocessor/
--rw-r--r--   0 mike      (1000) mike      (1000)     1012 2019-06-20 12:58:54.000000 gallery_dl-1.8.7/gallery_dl/postprocessor/__init__.py
--rw-r--r--   0 mike      (1000) mike      (1000)     1441 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/postprocessor/classify.py
--rw-r--r--   0 mike      (1000) mike      (1000)      584 2019-02-06 06:57:23.000000 gallery_dl-1.8.7/gallery_dl/postprocessor/common.py
--rw-r--r--   0 mike      (1000) mike      (1000)     1157 2019-06-03 18:07:04.000000 gallery_dl-1.8.7/gallery_dl/postprocessor/exec.py
--rw-r--r--   0 mike      (1000) mike      (1000)     1864 2019-06-03 18:07:05.000000 gallery_dl-1.8.7/gallery_dl/postprocessor/metadata.py
--rw-r--r--   0 mike      (1000) mike      (1000)     4723 2019-02-06 06:57:23.000000 gallery_dl-1.8.7/gallery_dl/postprocessor/ugoira.py
--rw-r--r--   0 mike      (1000) mike      (1000)     1964 2019-06-27 16:30:40.000000 gallery_dl-1.8.7/gallery_dl/postprocessor/zip.py
--rw-r--r--   0 mike      (1000) mike      (1000)     7502 2019-06-16 19:46:58.000000 gallery_dl-1.8.7/gallery_dl/text.py
--rw-r--r--   0 mike      (1000) mike      (1000)    19709 2019-06-27 16:30:41.000000 gallery_dl-1.8.7/gallery_dl/util.py
--rw-r--r--   0 mike      (1000) mike      (1000)      271 2019-06-28 18:54:16.000000 gallery_dl-1.8.7/gallery_dl/version.py
-drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2019-06-28 18:54:23.000000 gallery_dl-1.8.7/gallery_dl.egg-info/
--rw-r--r--   0 mike      (1000) mike      (1000)    10339 2019-06-28 18:54:20.000000 gallery_dl-1.8.7/gallery_dl.egg-info/PKG-INFO
--rw-r--r--   0 mike      (1000) mike      (1000)     4660 2019-06-28 18:54:20.000000 gallery_dl-1.8.7/gallery_dl.egg-info/SOURCES.txt
--rw-r--r--   0 mike      (1000) mike      (1000)        1 2019-06-28 18:54:20.000000 gallery_dl-1.8.7/gallery_dl.egg-info/dependency_links.txt
--rw-r--r--   0 mike      (1000) mike      (1000)       48 2019-06-28 18:54:20.000000 gallery_dl-1.8.7/gallery_dl.egg-info/entry_points.txt
--rw-r--r--   0 mike      (1000) mike      (1000)       17 2019-06-28 18:54:20.000000 gallery_dl-1.8.7/gallery_dl.egg-info/requires.txt
--rw-r--r--   0 mike      (1000) mike      (1000)       11 2019-06-28 18:54:20.000000 gallery_dl-1.8.7/gallery_dl.egg-info/top_level.txt
--rw-r--r--   0 mike      (1000) mike      (1000)      159 2019-06-28 18:54:23.000000 gallery_dl-1.8.7/setup.cfg
--rw-r--r--   0 mike      (1000) mike      (1000)     3783 2019-06-03 18:07:05.000000 gallery_dl-1.8.7/setup.py
-drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2019-06-28 18:54:23.000000 gallery_dl-1.8.7/test/
--rw-r--r--   0 mike      (1000) mike      (1000)     2731 2019-06-03 18:07:05.000000 gallery_dl-1.8.7/test/test_config.py
--rw-r--r--   0 mike      (1000) mike      (1000)     4133 2019-06-03 18:07:05.000000 gallery_dl-1.8.7/test/test_cookies.py
--rw-r--r--   0 mike      (1000) mike      (1000)     6874 2019-06-27 16:30:41.000000 gallery_dl-1.8.7/test/test_downloader.py
--rw-r--r--   0 mike      (1000) mike      (1000)     6285 2019-06-03 18:07:05.000000 gallery_dl-1.8.7/test/test_extractor.py
--rw-r--r--   0 mike      (1000) mike      (1000)     3489 2019-02-06 06:57:23.000000 gallery_dl-1.8.7/test/test_oauth.py
--rw-r--r--   0 mike      (1000) mike      (1000)    11059 2019-06-28 14:57:39.000000 gallery_dl-1.8.7/test/test_results.py
--rw-r--r--   0 mike      (1000) mike      (1000)    14049 2019-06-16 19:42:35.000000 gallery_dl-1.8.7/test/test_text.py
--rw-r--r--   0 mike      (1000) mike      (1000)    13354 2019-06-27 16:30:41.000000 gallery_dl-1.8.7/test/test_util.py
+drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2019-07-19 19:42:17.000000 gallery_dl-1.9.0/
+-rw-r--r--   0 mike      (1000) mike      (1000)    10442 2019-07-19 19:42:17.000000 gallery_dl-1.9.0/PKG-INFO
+-rw-r--r--   0 mike      (1000) mike      (1000)     7233 2019-07-19 19:42:12.000000 gallery_dl-1.9.0/README.rst
+-rw-r--r--   0 mike      (1000) mike      (1000)     5151 2019-07-19 19:42:05.000000 gallery_dl-1.9.0/gallery-dl.1
+-rw-r--r--   0 mike      (1000) mike      (1000)     1060 2019-07-19 19:42:06.000000 gallery_dl-1.9.0/gallery-dl.bash_completion
+-rw-r--r--   0 mike      (1000) mike      (1000)    41600 2019-07-19 19:42:05.000000 gallery_dl-1.9.0/gallery-dl.conf.5
+drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2019-07-19 19:42:17.000000 gallery_dl-1.9.0/gallery_dl/
+-rw-r--r--   0 mike      (1000) mike      (1000)     8613 2019-07-18 10:46:23.000000 gallery_dl-1.9.0/gallery_dl/__init__.py
+-rw-r--r--   0 mike      (1000) mike      (1000)      540 2019-02-19 14:28:59.000000 gallery_dl-1.9.0/gallery_dl/__main__.py
+-rw-r--r--   0 mike      (1000) mike      (1000)    12048 2019-06-03 18:07:03.000000 gallery_dl-1.9.0/gallery_dl/aes.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     5744 2019-06-20 13:36:46.000000 gallery_dl-1.9.0/gallery_dl/cache.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     5827 2019-06-03 18:07:03.000000 gallery_dl-1.9.0/gallery_dl/cloudflare.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     3915 2019-07-05 21:16:55.000000 gallery_dl-1.9.0/gallery_dl/config.py
+drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2019-07-19 19:42:17.000000 gallery_dl-1.9.0/gallery_dl/downloader/
+-rw-r--r--   0 mike      (1000) mike      (1000)     1048 2019-07-18 10:46:23.000000 gallery_dl-1.9.0/gallery_dl/downloader/__init__.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     1149 2019-07-18 10:46:23.000000 gallery_dl-1.9.0/gallery_dl/downloader/common.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     7737 2019-07-18 10:46:23.000000 gallery_dl-1.9.0/gallery_dl/downloader/http.py
+-rw-r--r--   0 mike      (1000) mike      (1000)      664 2019-07-18 10:46:23.000000 gallery_dl-1.9.0/gallery_dl/downloader/text.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     2901 2019-07-18 10:46:23.000000 gallery_dl-1.9.0/gallery_dl/downloader/ytdl.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     1898 2019-02-06 06:57:23.000000 gallery_dl-1.9.0/gallery_dl/exception.py
+drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2019-07-19 19:42:17.000000 gallery_dl-1.9.0/gallery_dl/extractor/
+-rw-r--r--   0 mike      (1000) mike      (1000)     3255 2019-06-03 18:07:03.000000 gallery_dl-1.9.0/gallery_dl/extractor/2chan.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     7138 2019-07-18 10:46:23.000000 gallery_dl-1.9.0/gallery_dl/extractor/35photo.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     3072 2019-06-03 18:07:03.000000 gallery_dl-1.9.0/gallery_dl/extractor/3dbooru.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     1357 2019-06-03 18:07:03.000000 gallery_dl-1.9.0/gallery_dl/extractor/4chan.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     7760 2019-07-19 13:37:40.000000 gallery_dl-1.9.0/gallery_dl/extractor/500px.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     1087 2019-06-03 18:07:03.000000 gallery_dl-1.9.0/gallery_dl/extractor/8chan.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     4604 2019-06-14 10:19:24.000000 gallery_dl-1.9.0/gallery_dl/extractor/8muses.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     3787 2019-07-19 11:20:37.000000 gallery_dl-1.9.0/gallery_dl/extractor/__init__.py
+-rw-r--r--   0 mike      (1000) mike      (1000)    13192 2019-07-18 10:46:23.000000 gallery_dl-1.9.0/gallery_dl/extractor/artstation.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     6219 2019-06-03 18:07:03.000000 gallery_dl-1.9.0/gallery_dl/extractor/behance.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     3912 2019-06-03 18:07:03.000000 gallery_dl-1.9.0/gallery_dl/extractor/bobx.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     7965 2019-06-03 18:07:03.000000 gallery_dl-1.9.0/gallery_dl/extractor/booru.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     2090 2019-06-03 18:07:03.000000 gallery_dl-1.9.0/gallery_dl/extractor/chan.py
+-rw-r--r--   0 mike      (1000) mike      (1000)    15520 2019-07-19 15:11:18.000000 gallery_dl-1.9.0/gallery_dl/extractor/common.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     3112 2019-06-03 18:07:03.000000 gallery_dl-1.9.0/gallery_dl/extractor/danbooru.py
+-rw-r--r--   0 mike      (1000) mike      (1000)    37053 2019-07-19 15:58:22.000000 gallery_dl-1.9.0/gallery_dl/extractor/deviantart.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     2166 2019-06-03 18:07:03.000000 gallery_dl-1.9.0/gallery_dl/extractor/directlink.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     5033 2019-06-03 18:07:03.000000 gallery_dl-1.9.0/gallery_dl/extractor/dynastyscans.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     2510 2019-06-03 18:07:03.000000 gallery_dl-1.9.0/gallery_dl/extractor/e621.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     2424 2019-07-18 10:46:23.000000 gallery_dl-1.9.0/gallery_dl/extractor/erolord.py
+-rw-r--r--   0 mike      (1000) mike      (1000)    13795 2019-07-18 10:46:23.000000 gallery_dl-1.9.0/gallery_dl/extractor/exhentai.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     3889 2019-06-03 18:07:03.000000 gallery_dl-1.9.0/gallery_dl/extractor/fallenangels.py
+-rw-r--r--   0 mike      (1000) mike      (1000)    18538 2019-06-03 18:07:03.000000 gallery_dl-1.9.0/gallery_dl/extractor/flickr.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     5395 2019-06-03 18:07:03.000000 gallery_dl-1.9.0/gallery_dl/extractor/foolfuuka.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     9025 2019-06-03 18:07:03.000000 gallery_dl-1.9.0/gallery_dl/extractor/foolslide.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     4720 2019-06-03 18:07:03.000000 gallery_dl-1.9.0/gallery_dl/extractor/gelbooru.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     2933 2019-06-03 18:07:03.000000 gallery_dl-1.9.0/gallery_dl/extractor/gfycat.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     3843 2019-06-03 18:07:03.000000 gallery_dl-1.9.0/gallery_dl/extractor/hbrowse.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     3800 2019-06-03 18:07:03.000000 gallery_dl-1.9.0/gallery_dl/extractor/hentai2read.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     3200 2019-06-27 16:30:40.000000 gallery_dl-1.9.0/gallery_dl/extractor/hentaicafe.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     9967 2019-06-27 16:30:40.000000 gallery_dl-1.9.0/gallery_dl/extractor/hentaifoundry.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     4417 2019-06-03 18:07:03.000000 gallery_dl-1.9.0/gallery_dl/extractor/hentaifox.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     3843 2019-06-03 18:07:03.000000 gallery_dl-1.9.0/gallery_dl/extractor/hentaihere.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     3695 2019-06-03 18:07:03.000000 gallery_dl-1.9.0/gallery_dl/extractor/hentainexus.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     3956 2019-06-27 18:24:42.000000 gallery_dl-1.9.0/gallery_dl/extractor/hitomi.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     2527 2019-06-03 18:07:03.000000 gallery_dl-1.9.0/gallery_dl/extractor/hypnohub.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     2148 2019-06-03 18:07:03.000000 gallery_dl-1.9.0/gallery_dl/extractor/idolcomplex.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     4771 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/imagebam.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     7400 2019-06-27 16:30:40.000000 gallery_dl-1.9.0/gallery_dl/extractor/imagefap.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     9146 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/imagehosts.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     4561 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/imgbox.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     2292 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/imgth.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     6596 2019-07-18 10:46:23.000000 gallery_dl-1.9.0/gallery_dl/extractor/imgur.py
+-rw-r--r--   0 mike      (1000) mike      (1000)    11546 2019-07-18 10:46:23.000000 gallery_dl-1.9.0/gallery_dl/extractor/instagram.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     5315 2019-06-27 16:30:40.000000 gallery_dl-1.9.0/gallery_dl/extractor/keenspot.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     2852 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/khinsider.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     8187 2019-06-28 18:40:54.000000 gallery_dl-1.9.0/gallery_dl/extractor/kissmanga.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     4134 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/komikcast.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     3035 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/konachan.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     5318 2019-06-06 08:45:38.000000 gallery_dl-1.9.0/gallery_dl/extractor/livedoor.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     8191 2019-07-12 17:42:14.000000 gallery_dl-1.9.0/gallery_dl/extractor/luscious.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     6336 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/mangadex.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     2292 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/mangafox.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     5160 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/mangahere.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     1377 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/mangapanda.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     5358 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/mangapark.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     4673 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/mangareader.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     1995 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/mangastream.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     5902 2019-06-27 16:30:40.000000 gallery_dl-1.9.0/gallery_dl/extractor/mangoxo.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     6696 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/mastodon.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     1800 2019-03-14 21:16:42.000000 gallery_dl-1.9.0/gallery_dl/extractor/message.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     3445 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/myportfolio.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     5628 2019-07-19 12:34:08.000000 gallery_dl-1.9.0/gallery_dl/extractor/newgrounds.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     1661 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/ngomik.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     4505 2019-06-17 18:01:25.000000 gallery_dl-1.9.0/gallery_dl/extractor/nhentai.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     7160 2019-07-18 10:46:23.000000 gallery_dl-1.9.0/gallery_dl/extractor/nijie.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     2254 2019-06-27 16:30:40.000000 gallery_dl-1.9.0/gallery_dl/extractor/nsfwalbum.py
+-rw-r--r--   0 mike      (1000) mike      (1000)    11257 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/oauth.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     4142 2019-06-05 09:39:49.000000 gallery_dl-1.9.0/gallery_dl/extractor/paheal.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     6219 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/patreon.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     6725 2019-06-10 12:58:39.000000 gallery_dl-1.9.0/gallery_dl/extractor/photobucket.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     3917 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/piczel.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     8887 2019-07-18 10:46:23.000000 gallery_dl-1.9.0/gallery_dl/extractor/pinterest.py
+-rw-r--r--   0 mike      (1000) mike      (1000)    18118 2019-07-18 10:46:23.000000 gallery_dl-1.9.0/gallery_dl/extractor/pixiv.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     6597 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/pixnet.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     4123 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/plurk.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     5415 2019-06-07 14:27:33.000000 gallery_dl-1.9.0/gallery_dl/extractor/pornhub.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     3795 2019-06-27 16:30:40.000000 gallery_dl-1.9.0/gallery_dl/extractor/pururin.py
+-rw-r--r--   0 mike      (1000) mike      (1000)    11643 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/reactor.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     3598 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/readcomiconline.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     1672 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/recursive.py
+-rw-r--r--   0 mike      (1000) mike      (1000)    11487 2019-07-18 10:46:23.000000 gallery_dl-1.9.0/gallery_dl/extractor/reddit.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     2385 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/rule34.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     2453 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/safebooru.py
+-rw-r--r--   0 mike      (1000) mike      (1000)    10524 2019-07-05 13:51:48.000000 gallery_dl-1.9.0/gallery_dl/extractor/sankaku.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     4143 2019-07-18 10:46:23.000000 gallery_dl-1.9.0/gallery_dl/extractor/sankakucomplex.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     7035 2019-07-18 10:46:23.000000 gallery_dl-1.9.0/gallery_dl/extractor/seiga.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     2500 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/senmanga.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     7479 2019-07-18 10:46:23.000000 gallery_dl-1.9.0/gallery_dl/extractor/sexcom.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     4222 2019-07-18 10:46:23.000000 gallery_dl-1.9.0/gallery_dl/extractor/shopify.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     7244 2019-07-18 10:46:23.000000 gallery_dl-1.9.0/gallery_dl/extractor/simplyhentai.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     4550 2019-06-14 16:40:11.000000 gallery_dl-1.9.0/gallery_dl/extractor/slickpic.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     3329 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/slideshare.py
+-rw-r--r--   0 mike      (1000) mike      (1000)    10570 2019-07-19 12:30:18.000000 gallery_dl-1.9.0/gallery_dl/extractor/smugmug.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     2488 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/test.py
+-rw-r--r--   0 mike      (1000) mike      (1000)    11744 2019-07-18 10:46:23.000000 gallery_dl-1.9.0/gallery_dl/extractor/tsumino.py
+-rw-r--r--   0 mike      (1000) mike      (1000)    14891 2019-07-19 12:36:27.000000 gallery_dl-1.9.0/gallery_dl/extractor/tumblr.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     8160 2019-07-18 10:46:23.000000 gallery_dl-1.9.0/gallery_dl/extractor/twitter.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     3368 2019-06-27 16:30:40.000000 gallery_dl-1.9.0/gallery_dl/extractor/vanillarock.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     5173 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/wallhaven.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     4054 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/warosu.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     4641 2019-06-22 18:50:48.000000 gallery_dl-1.9.0/gallery_dl/extractor/weibo.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     4395 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/wikiart.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     5927 2019-06-06 20:36:49.000000 gallery_dl-1.9.0/gallery_dl/extractor/xhamster.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     4841 2019-07-18 10:46:23.000000 gallery_dl-1.9.0/gallery_dl/extractor/xvideos.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     2413 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/yandere.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     4021 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/yaplog.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     4549 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/extractor/yuki.py
+-rw-r--r--   0 mike      (1000) mike      (1000)    17068 2019-07-18 10:46:23.000000 gallery_dl-1.9.0/gallery_dl/job.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     4189 2019-07-18 10:46:23.000000 gallery_dl-1.9.0/gallery_dl/oauth.py
+-rw-r--r--   0 mike      (1000) mike      (1000)    11925 2019-07-18 10:46:24.000000 gallery_dl-1.9.0/gallery_dl/option.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     7239 2019-07-18 10:46:24.000000 gallery_dl-1.9.0/gallery_dl/output.py
+drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2019-07-19 19:42:17.000000 gallery_dl-1.9.0/gallery_dl/postprocessor/
+-rw-r--r--   0 mike      (1000) mike      (1000)      996 2019-07-18 10:46:24.000000 gallery_dl-1.9.0/gallery_dl/postprocessor/__init__.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     1441 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/postprocessor/classify.py
+-rw-r--r--   0 mike      (1000) mike      (1000)      584 2019-02-06 06:57:23.000000 gallery_dl-1.9.0/gallery_dl/postprocessor/common.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     1157 2019-06-03 18:07:04.000000 gallery_dl-1.9.0/gallery_dl/postprocessor/exec.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     1864 2019-07-15 13:31:07.000000 gallery_dl-1.9.0/gallery_dl/postprocessor/metadata.py
+-rw-r--r--   0 mike      (1000) mike      (1000)      734 2019-07-18 10:46:24.000000 gallery_dl-1.9.0/gallery_dl/postprocessor/mtime.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     4723 2019-02-06 06:57:23.000000 gallery_dl-1.9.0/gallery_dl/postprocessor/ugoira.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     1964 2019-06-27 16:30:40.000000 gallery_dl-1.9.0/gallery_dl/postprocessor/zip.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     7575 2019-07-18 10:46:24.000000 gallery_dl-1.9.0/gallery_dl/text.py
+-rw-r--r--   0 mike      (1000) mike      (1000)    20332 2019-07-18 10:46:24.000000 gallery_dl-1.9.0/gallery_dl/util.py
+-rw-r--r--   0 mike      (1000) mike      (1000)      271 2019-07-19 19:42:12.000000 gallery_dl-1.9.0/gallery_dl/version.py
+drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2019-07-19 19:42:17.000000 gallery_dl-1.9.0/gallery_dl.egg-info/
+-rw-r--r--   0 mike      (1000) mike      (1000)    10442 2019-07-19 19:42:16.000000 gallery_dl-1.9.0/gallery_dl.egg-info/PKG-INFO
+-rw-r--r--   0 mike      (1000) mike      (1000)     4726 2019-07-19 19:42:16.000000 gallery_dl-1.9.0/gallery_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 mike      (1000) mike      (1000)        1 2019-07-19 19:42:16.000000 gallery_dl-1.9.0/gallery_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 mike      (1000) mike      (1000)       48 2019-07-19 19:42:16.000000 gallery_dl-1.9.0/gallery_dl.egg-info/entry_points.txt
+-rw-r--r--   0 mike      (1000) mike      (1000)       17 2019-07-19 19:42:16.000000 gallery_dl-1.9.0/gallery_dl.egg-info/requires.txt
+-rw-r--r--   0 mike      (1000) mike      (1000)       11 2019-07-19 19:42:16.000000 gallery_dl-1.9.0/gallery_dl.egg-info/top_level.txt
+-rw-r--r--   0 mike      (1000) mike      (1000)      159 2019-07-19 19:42:17.000000 gallery_dl-1.9.0/setup.cfg
+-rw-r--r--   0 mike      (1000) mike      (1000)     3783 2019-06-03 18:07:05.000000 gallery_dl-1.9.0/setup.py
+drwxr-xr-x   0 mike      (1000) mike      (1000)        0 2019-07-19 19:42:17.000000 gallery_dl-1.9.0/test/
+-rw-r--r--   0 mike      (1000) mike      (1000)     2731 2019-06-03 18:07:05.000000 gallery_dl-1.9.0/test/test_config.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     4133 2019-06-03 18:07:05.000000 gallery_dl-1.9.0/test/test_cookies.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     9050 2019-07-19 11:21:35.000000 gallery_dl-1.9.0/test/test_downloader.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     6285 2019-06-03 18:07:05.000000 gallery_dl-1.9.0/test/test_extractor.py
+-rw-r--r--   0 mike      (1000) mike      (1000)     3489 2019-02-06 06:57:23.000000 gallery_dl-1.9.0/test/test_oauth.py
+-rw-r--r--   0 mike      (1000) mike      (1000)    11166 2019-07-19 19:40:15.000000 gallery_dl-1.9.0/test/test_results.py
+-rw-r--r--   0 mike      (1000) mike      (1000)    14049 2019-07-17 12:26:02.000000 gallery_dl-1.9.0/test/test_text.py
+-rw-r--r--   0 mike      (1000) mike      (1000)    13354 2019-06-27 16:30:41.000000 gallery_dl-1.9.0/test/test_util.py
```

### Comparing `gallery_dl-1.8.7/PKG-INFO` & `gallery_dl-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: gallery_dl
-Version: 1.8.7
+Version: 1.9.0
 Summary: Command-line program to download image-galleries and -collections from several image hosting sites
 Home-page: https://github.com/mikf/gallery-dl
 Author: Mike Fährmann
 Author-email: mike_faehrmann@web.de
 Maintainer: Mike Fährmann
 Maintainer-email: mike_faehrmann@web.de
 License: GPLv2
@@ -29,14 +29,15 @@
         - Requests_
         
         Optional
         --------
         
         - FFmpeg_: Pixiv Ugoira to WebM conversion
         - youtube-dl_: Video downloads
+        - pyOpenSSL_: Access Cloudflare protected sites
         
         
         Installation
         ============
         
         Pip
         ---
@@ -84,16 +85,16 @@
         Standalone Executable
         ---------------------
         
         Download a standalone executable file,
         put it into your `PATH <https://en.wikipedia.org/wiki/PATH_(variable)>`__,
         and run it inside a command prompt (like ``cmd.exe``).
         
-        - `Windows <https://github.com/mikf/gallery-dl/releases/download/v1.8.7/gallery-dl.exe>`__
-        - `Linux   <https://github.com/mikf/gallery-dl/releases/download/v1.8.7/gallery-dl.bin>`__
+        - `Windows <https://github.com/mikf/gallery-dl/releases/download/v1.9.0/gallery-dl.exe>`__
+        - `Linux   <https://github.com/mikf/gallery-dl/releases/download/v1.9.0/gallery-dl.bin>`__
         
         These executables include a Python 3.7 interpreter
         and all required Python packages.
         
         
         Snap
         ----
@@ -229,23 +230,24 @@
         "tokens", which should be added to your configuration file.
         
         
         .. _gallery-dl.conf:         https://github.com/mikf/gallery-dl/blob/master/docs/gallery-dl.conf
         .. _gallery-dl-example.conf: https://github.com/mikf/gallery-dl/blob/master/docs/gallery-dl-example.conf
         .. _configuration.rst:       https://github.com/mikf/gallery-dl/blob/master/docs/configuration.rst
         .. _Supported Sites:         https://github.com/mikf/gallery-dl/blob/master/docs/supportedsites.rst
-        .. _stable:                  https://github.com/mikf/gallery-dl/archive/v1.8.7.zip
+        .. _stable:                  https://github.com/mikf/gallery-dl/archive/v1.9.0.zip
         .. _dev:                     https://github.com/mikf/gallery-dl/archive/master.zip
         
         .. _Python:     https://www.python.org/downloads/
         .. _PyPI:       https://pypi.org/
         .. _pip:        https://pip.pypa.io/en/stable/
         .. _Requests:   http://docs.python-requests.org/en/master/
         .. _FFmpeg:     https://www.ffmpeg.org/
         .. _youtube-dl: https://ytdl-org.github.io/youtube-dl/
+        .. _pyOpenSSL:  https://pyopenssl.org/
         .. _Snapd:      https://docs.snapcraft.io/installing-snapd
         .. _OAuth:      https://en.wikipedia.org/wiki/OAuth
         
         .. |pypi| image:: https://img.shields.io/pypi/v/gallery-dl.svg
             :target: https://pypi.org/project/gallery-dl/
         
         .. |build| image:: https://travis-ci.org/mikf/gallery-dl.svg?branch=master
```

### Comparing `gallery_dl-1.8.7/README.rst` & `gallery_dl-1.9.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 - Requests_
 
 Optional
 --------
 
 - FFmpeg_: Pixiv Ugoira to WebM conversion
 - youtube-dl_: Video downloads
+- pyOpenSSL_: Access Cloudflare protected sites
 
 
 Installation
 ============
 
 Pip
 ---
@@ -73,16 +74,16 @@
 Standalone Executable
 ---------------------
 
 Download a standalone executable file,
 put it into your `PATH <https://en.wikipedia.org/wiki/PATH_(variable)>`__,
 and run it inside a command prompt (like ``cmd.exe``).
 
-- `Windows <https://github.com/mikf/gallery-dl/releases/download/v1.8.7/gallery-dl.exe>`__
-- `Linux   <https://github.com/mikf/gallery-dl/releases/download/v1.8.7/gallery-dl.bin>`__
+- `Windows <https://github.com/mikf/gallery-dl/releases/download/v1.9.0/gallery-dl.exe>`__
+- `Linux   <https://github.com/mikf/gallery-dl/releases/download/v1.9.0/gallery-dl.bin>`__
 
 These executables include a Python 3.7 interpreter
 and all required Python packages.
 
 
 Snap
 ----
@@ -218,23 +219,24 @@
 "tokens", which should be added to your configuration file.
 
 
 .. _gallery-dl.conf:         https://github.com/mikf/gallery-dl/blob/master/docs/gallery-dl.conf
 .. _gallery-dl-example.conf: https://github.com/mikf/gallery-dl/blob/master/docs/gallery-dl-example.conf
 .. _configuration.rst:       https://github.com/mikf/gallery-dl/blob/master/docs/configuration.rst
 .. _Supported Sites:         https://github.com/mikf/gallery-dl/blob/master/docs/supportedsites.rst
-.. _stable:                  https://github.com/mikf/gallery-dl/archive/v1.8.7.zip
+.. _stable:                  https://github.com/mikf/gallery-dl/archive/v1.9.0.zip
 .. _dev:                     https://github.com/mikf/gallery-dl/archive/master.zip
 
 .. _Python:     https://www.python.org/downloads/
 .. _PyPI:       https://pypi.org/
 .. _pip:        https://pip.pypa.io/en/stable/
 .. _Requests:   http://docs.python-requests.org/en/master/
 .. _FFmpeg:     https://www.ffmpeg.org/
 .. _youtube-dl: https://ytdl-org.github.io/youtube-dl/
+.. _pyOpenSSL:  https://pyopenssl.org/
 .. _Snapd:      https://docs.snapcraft.io/installing-snapd
 .. _OAuth:      https://en.wikipedia.org/wiki/OAuth
 
 .. |pypi| image:: https://img.shields.io/pypi/v/gallery-dl.svg
     :target: https://pypi.org/project/gallery-dl/
 
 .. |build| image:: https://travis-ci.org/mikf/gallery-dl.svg?branch=master
```

### Comparing `gallery_dl-1.8.7/gallery-dl.1` & `gallery_dl-1.9.0/gallery-dl.1`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "GALLERY-DL" "1" "2019-06-28" "1.8.7-dev" "gallery-dl Manual"
+.TH "GALLERY-DL" "1" "2019-07-19" "1.9.0-dev" "gallery-dl Manual"
 .\" disable hyphenation
 .nh
 
 .SH NAME
 gallery-dl \- download image-galleries and -collections
 
 .SH SYNOPSIS
@@ -67,32 +67,38 @@
 .TP
 .B "\-\-write\-unsupported" \f[I]FILE\f[]
 Write URLs, which get emitted by other extractors but cannot be handled, to FILE
 .TP
 .B "\-r, \-\-limit\-rate" \f[I]RATE\f[]
 Maximum download rate (e.g. 500k or 2.5M)
 .TP
-.B "\-R, \-\-retries" \f[I]RETRIES\f[]
-Number of retries (default: 5)
+.B "\-R, \-\-retries" \f[I]N\f[]
+Maximum number of retries for failed HTTP requests or -1 for infinite retries (default: 4)
+.TP
+.B "\-A, \-\-abort" \f[I]N\f[]
+Abort extractor run after N consecutive file downloads have been skipped, e.g. if files with the same filename already exist
 .TP
 .B "\-\-http\-timeout" \f[I]SECONDS\f[]
 Timeout for HTTP connections (defaut: 30.0)
 .TP
 .B "\-\-sleep" \f[I]SECONDS\f[]
 Number of seconds to sleep before each download
 .TP
 .B "\-\-no\-part" 
 Do not use .part files
 .TP
+.B "\-\-no\-mtime" 
+Do not set file modification times according to Last-Modified HTTP response headers
+.TP
+.B "\-\-no\-download" 
+Do not download any files
+.TP
 .B "\-\-no\-check\-certificate" 
 Disable HTTPS certificate validation
 .TP
-.B "\-\-abort\-on\-skip" 
-Abort extractor run if a file download would normally be skipped, i.e. if a file with the same filename already exists
-.TP
 .B "\-c, \-\-config" \f[I]FILE\f[]
 Additional configuration files
 .TP
 .B "\-o, \-\-option" \f[I]OPT\f[]
 Additional '<key>=<value>' option values
 .TP
 .B "\-\-ignore\-config" 
@@ -129,14 +135,17 @@
 Convert Pixiv Ugoira to WebM (requires FFmpeg)
 .TP
 .B "\-\-write\-metadata" 
 Write metadata to separate JSON files
 .TP
 .B "\-\-write\-tags" 
 Write image tags to separate text files
+.TP
+.B "\-\-mtime\-from\-date" 
+Set file modification times according to 'date' metadata
 
 .SH EXAMPLES
 .TP
 gallery-dl \f[I]URL\f[]
 Download images from \f[I]URL\f[].
 .TP
 gallery-dl -g -u <username> -p <password> \f[I]URL\f[]
```

### Comparing `gallery_dl-1.8.7/gallery-dl.bash_completion` & `gallery_dl-1.9.0/gallery-dl.bash_completion`

 * *Files 6% similar despite different names*

```diff
@@ -6,12 +6,12 @@
     prev="${COMP_WORDS[COMP_CWORD-1]}"
 
     if [[ "${prev}" =~ ^(-i|--input-file|--cookies|--write-log|--write-unsupported|-c|--config|--config-yaml|--download-archive)$ ]]; then
         COMPREPLY=( $(compgen -f -- "${cur}") )
     elif [[ "${prev}" =~ ^(-d|--dest)$ ]]; then
         COMPREPLY=( $(compgen -d -- "${cur}") )
     else
-        COMPREPLY=( $(compgen -W "--help --version --dest --input-file --cookies --proxy --clear-cache --quiet --verbose --get-urls --dump-json --simulate --list-keywords --list-modules --list-extractors --write-log --write-unsupported --limit-rate --retries --http-timeout --sleep --no-part --no-check-certificate --abort-on-skip --config --config-yaml --option --ignore-config --username --password --netrc --download-archive --range --chapter-range --filter --chapter-filter --zip --ugoira-conv --write-metadata --write-tags" -- "${cur}") )
+        COMPREPLY=( $(compgen -W "--help --version --dest --input-file --cookies --proxy --clear-cache --quiet --verbose --get-urls --dump-json --simulate --list-keywords --list-modules --list-extractors --write-log --write-unsupported --limit-rate --retries --abort --http-timeout --sleep --no-part --no-mtime --no-download --no-check-certificate --abort-on-skip --config --config-yaml --option --ignore-config --username --password --netrc --download-archive --range --chapter-range --filter --chapter-filter --zip --ugoira-conv --write-metadata --write-tags --mtime-from-date" -- "${cur}") )
     fi
 }
 
 complete -F _gallery_dl gallery-dl
```

### Comparing `gallery_dl-1.8.7/gallery-dl.conf.5` & `gallery_dl-1.9.0/gallery-dl.conf.5`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH "GALLERY-DL.CONF" "5" "2019-06-28" "1.8.7-dev" "gallery-dl Manual"
+.TH "GALLERY-DL.CONF" "5" "2019-07-19" "1.9.0-dev" "gallery-dl Manual"
 .\" disable hyphenation
 .nh
 .\" disable justification (adjust text to left margin only)
 .ad l
 
 .SH NAME
 gallery-dl.conf \- gallery-dl configuration file
@@ -261,15 +261,15 @@
 otherwise \f[I]http://\f[] is assumed.
 
 .SS extractor.*.user-agent
 .IP "Type:" 6
 \f[I]string\f[]
 
 .IP "Default:" 9
-\f[I]"Mozilla/5.0 (X11; Linux x86_64; rv:62.0) Gecko/20100101 Firefox/62.0"\f[]
+\f[I]"Mozilla/5.0 (X11; Linux x86_64; rv:68.0) Gecko/20100101 Firefox/68.0"\f[]
 
 .IP "Description:" 4
 User-Agent header value to be used for HTTP requests.
 
 Note: This option has no effect on pixiv and
 readcomiconline extractors, as these need specific values to
 function correctly.
@@ -351,18 +351,19 @@
 in the same order as they are specified.
 
 .SS extractor.*.retries
 .IP "Type:" 6
 \f[I]integer\f[]
 
 .IP "Default:" 9
-\f[I]5\f[]
+\f[I]4\f[]
 
 .IP "Description:" 4
-Number of times a failed HTTP request is retried before giving up.
+Maximum number of times a failed HTTP request is retried before
+giving up or \f[I]-1\f[] for infinite retries.
 
 .SS extractor.*.timeout
 .IP "Type:" 6
 \f[I]float\f[] or \f[I]null\f[]
 
 .IP "Default:" 9
 \f[I]30\f[]
@@ -386,14 +387,28 @@
 
 If this is a \f[I]string\f[], it must be the path to a CA bundle to use
 instead of the default certificates.
 
 This value gets internally used as the \f[I]verify\f[] parameter for the
 \f[I]requests.request()\f[] method.
 
+.SS extractor.*.download
+.IP "Type:" 6
+\f[I]bool\f[]
+
+.IP "Default:" 9
+\f[I]true\f[]
+
+.IP "Description:" 4
+Controls whether to download media files.
+
+Setting this to \f[I]false\f[] won't download any files, but all other
+functions (postprocessors_, \f[I]download archive\f[], etc.)
+will be executed as normal.
+
 .SS extractor.*.image-range
 .IP "Type:" 6
 \f[I]string\f[]
 
 .IP "Example:" 4
 "10-20",
 .br
@@ -437,14 +452,49 @@
 .IP "Type:" 6
 \f[I]string\f[]
 
 .IP "Description:" 4
 Like \f[I]image-filter\f[], but applies to delegated URLs
 like manga-chapters, etc.
 
+.SS extractor.*.image-unique
+.IP "Type:" 6
+\f[I]bool\f[]
+
+.IP "Default:" 9
+\f[I]false\f[]
+
+.IP "Description:" 4
+Ignore image URLs that have been encountered before during the
+current extractor run.
+
+.SS extractor.*.chapter-unique
+.IP "Type:" 6
+\f[I]bool\f[]
+
+.IP "Default:" 9
+\f[I]false\f[]
+
+.IP "Description:" 4
+Like \f[I]image-unique\f[], but applies to delegated URLs
+like manga-chapters, etc.
+
+.SS extractor.*.date-format
+.IP "Type:" 6
+\f[I]string\f[]
+
+.IP "Default:" 9
+\f[I]"%Y-%m-%dT%H:%M:%S"\f[]
+
+.IP "Description:" 4
+Format string used to parse \f[I]string\f[] values of
+date-min and date-max.
+
+See \f[I]strptime\f[] for a list of formatting directives.
+
 .SH EXTRACTOR-SPECIFIC OPTIONS
 .SS extractor.artstation.external
 .IP "Type:" 6
 \f[I]bool\f[]
 
 .IP "Default:" 9
 \f[I]false\f[]
@@ -833,40 +883,22 @@
 Retrieve additional comments by resolving the \f[I]more\f[] comment
 stubs in the base comment tree.
 
 This requires 1 additional API call for every 100 extra comments.
 
 .SS extractor.reddit.date-min & .date-max
 .IP "Type:" 6
-\f[I]integer\f[] or \f[I]string\f[]
+\f[I]Date\f[]
 
 .IP "Default:" 9
 \f[I]0\f[] and \f[I]253402210800\f[] (timestamp of \f[I]datetime.max\f[])
 
 .IP "Description:" 4
 Ignore all submissions posted before/after this date.
 
-
-* If this is an \f[I]integer\f[], it represents the date as UTC timestamp.
-
-* If this is a \f[I]string\f[], it will get parsed according to date-format_.
-
-.SS extractor.reddit.date-format
-.IP "Type:" 6
-\f[I]string\f[]
-
-.IP "Default:" 9
-\f[I]"%Y-%m-%dT%H:%M:%S"\f[]
-
-.IP "Description:" 4
-An explicit format string used to parse the \f[I]string\f[] values of
-\f[I]date-min and date-max\f[].
-
-See \f[I]strptime\f[] for a list of formatting directives.
-
 .SS extractor.reddit.id-min & .id-max
 .IP "Type:" 6
 \f[I]string\f[]
 
 .IP "Example:" 4
 "6kmzv2"
 
@@ -940,14 +972,24 @@
 
 .IP "Default:" 9
 \f[I]false\f[]
 
 .IP "Description:" 4
 Download blog avatars.
 
+.SS extractor.tumblr.date-min & .date-max
+.IP "Type:" 6
+\f[I]Date\f[]
+
+.IP "Default:" 9
+\f[I]0\f[] and \f[I]null\f[]
+
+.IP "Description:" 4
+Ignore all posts published before/after this date.
+
 .SS extractor.tumblr.external
 .IP "Type:" 6
 \f[I]bool\f[]
 
 .IP "Default:" 9
 \f[I]false\f[]
 
@@ -995,14 +1037,24 @@
 A (comma-separated) list of post types to extract images, etc. from.
 
 Possible types are \f[I]text\f[], \f[I]quote\f[], \f[I]link\f[], \f[I]answer\f[],
 \f[I]video\f[], \f[I]audio\f[], \f[I]photo\f[], \f[I]chat\f[].
 
 You can use \f[I]"all"\f[] instead of listing all types separately.
 
+.SS extractor.twitter.content
+.IP "Type:" 6
+\f[I]bool\f[]
+
+.IP "Default:" 9
+\f[I]false\f[]
+
+.IP "Description:" 4
+Extract tweet text as \f[I]content\f[] metadata.
+
 .SS extractor.twitter.retweets
 .IP "Type:" 6
 \f[I]bool\f[]
 
 .IP "Default:" 9
 \f[I]true\f[]
 
@@ -1067,14 +1119,25 @@
 
 .IP "Default:" 9
 \f[I]true\f[]
 
 .IP "Description:" 4
 Enable/Disable this downloader module.
 
+.SS downloader.*.mtime
+.IP "Type:" 6
+\f[I]bool\f[]
+
+.IP "Default:" 9
+\f[I]true\f[]
+
+.IP "Description:" 4
+Use \f[I]Last-Modified\f[] HTTP response headers
+to set file modification times.
+
 .SS downloader.*.part
 .IP "Type:" 6
 \f[I]bool\f[]
 
 .IP "Default:" 9
 \f[I]true\f[]
 
@@ -1124,15 +1187,16 @@
 .IP "Type:" 6
 \f[I]integer\f[]
 
 .IP "Default:" 9
 \f[I]extractor.*.retries\f[]
 
 .IP "Description:" 4
-Number of retries during file downloads.
+Maximum number of retries during file downloads
+or \f[I]-1\f[] for infinite retries.
 
 .SS downloader.*.timeout
 .IP "Type:" 6
 \f[I]float\f[] or \f[I]null\f[]
 
 .IP "Default:" 9
 \f[I]extractor.*.timeout\f[]
@@ -1383,14 +1447,27 @@
 "tags:\\n\\n{tags:J\\n}\\n"
 
 .IP "Description:" 4
 Custom format string to build content of metadata files.
 
 Note: Only applies for \f[I]"mode": "custom"\f[].
 
+.SS mtime.key
+.IP "Type:" 6
+\f[I]string\f[]
+
+.IP "Default:" 9
+\f[I]"date"\f[]
+
+.IP "Description:" 4
+Name of the metadata field whose value should be used.
+
+This value must either be a UNIX timestamp or a
+\f[I]datetime\f[] object.
+
 .SS ugoira.extension
 .IP "Type:" 6
 \f[I]string\f[]
 
 .IP "Default:" 9
 \f[I]"webm"\f[]
 
@@ -1530,14 +1607,31 @@
 .IP "Description:" 4
 Path of the SQLite3 database used to cache login sessions,
 cookies and API tokens across gallery-dl invocations.
 
 Set this option to \f[I]null\f[] or an invalid path to disable
 this cache.
 
+.SS ciphers
+.IP "Type:" 6
+\f[I]bool\f[] or \f[I]string\f[]
+
+.IP "Default:" 9
+\f[I]true\f[]
+
+.IP "Description:" 4
+
+* \f[I]true\f[]: Update urllib3's default cipher list
+
+* \f[I]false\f[]: Leave the default cipher list as is
+
+* Any \f[I]string\f[]: Replace urllib3's default ciphers with these
+(See \f[I]SSLContext.set_ciphers() <https://docs.python.org/3/library/ssl.html#ssl.SSLContext.set_ciphers>\f[]
+for details)
+
 .SH API TOKENS & IDS
 .SS extractor.deviantart.client-id & .client-secret
 .IP "Type:" 6
 \f[I]string\f[]
 
 .IP "How To:" 4
 
@@ -1639,14 +1733,34 @@
 
 * click "Show secret key" (below "OAuth Consumer Key")
 
 * copy your \f[I]OAuth Consumer Key\f[] and \f[I]Secret Key\f[]
 and put them in your configuration file
 
 .SH CUSTOM TYPES
+.SS Date
+.IP "Type:" 6
+\f[I]string\f[] or \f[I]integer\f[]
+
+.IP "Examples:" 4
+
+* \f[I]"2019-01-01T00:00:00"\f[]
+
+* \f[I]"2019"\f[] with \f[I]"%Y"\f[] as \f[I]date-format\f[]
+
+* \f[I]1546297200\f[]
+
+.IP "Description:" 4
+A \f[I]Date\f[] value represents a specific point in time.
+
+
+* If given as \f[I]string\f[], it is parsed according to date-format_.
+
+* If given as \f[I]integer\f[], it is interpreted as UTC timestamp.
+
 .SS Path
 .IP "Type:" 6
 \f[I]string\f[] or \f[I]list\f[] of \f[I]strings\f[]
 
 .IP "Examples:" 4
 
 * \f[I]"file.ext"\f[]
@@ -1673,32 +1787,43 @@
 \f[I]"C:\\\\path\\\\to\\\\file.ext"\f[] if you want to use backslashes.
 
 .SS Logging Configuration
 .IP "Type:" 6
 \f[I]object\f[]
 
 
-.IP "Example:" 4
+.IP "Examples:" 4
 .. code::
 
 {
 "format": "{asctime} {name}: {message}",
 "format-date": "%H:%M:%S",
 "path": "~/log.txt",
 "encoding": "ascii"
 }
 
+{
+"level": "debug",
+"format": {
+"debug"  : "debug: {message}",
+"info"   : "[{name}] {message}",
+"warning": "Warning: {message}",
+"error"  : "ERROR: {message}"
+}
+}
+
 
 .IP "Description:" 4
 Extended logging output configuration.
 
 
 * format
 
-* Format string for logging messages
+* General format string for logging messages
+or a dictionary with format strings for each loglevel.
 
 In addition to the default
 \f[I]LogRecord attributes <https://docs.python.org/3/library/logging.html#logrecord-attributes>\f[],
 it is also possible to access the current
 \f[I]extractor <https://github.com/mikf/gallery-dl/blob/2e516a1e3e09cb8a9e36a8f6f7e41ce8d4402f5a/gallery_dl/extractor/common.py#L24>\f[]
 and \f[I]job <https://github.com/mikf/gallery-dl/blob/2e516a1e3e09cb8a9e36a8f6f7e41ce8d4402f5a/gallery_dl/job.py#L19>\f[]
 objects as well as their attributes
```

### Comparing `gallery_dl-1.8.7/gallery_dl/__init__.py` & `gallery_dl-1.9.0/gallery_dl/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,15 +118,17 @@
         if args.load_config:
             config.load()
         if args.cfgfiles:
             config.load(args.cfgfiles, strict=True)
         if args.yamlfiles:
             config.load(args.yamlfiles, strict=True, fmt="yaml")
         if args.postprocessors:
-            config.set(("postprocessors", ), args.postprocessors)
+            config.set(("postprocessors",), args.postprocessors)
+        if args.abort:
+            config.set(("skip",), "abort:" + str(args.abort))
         for key, value in args.options:
             config.set(key, value)
 
         # stream logging handler
         output.configure_logging_handler(
             "log", logging.getLogger().handlers[0])
```

### Comparing `gallery_dl-1.8.7/gallery_dl/__main__.py` & `gallery_dl-1.9.0/gallery_dl/__main__.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/aes.py` & `gallery_dl-1.9.0/gallery_dl/aes.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/cache.py` & `gallery_dl-1.9.0/gallery_dl/cache.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/cloudflare.py` & `gallery_dl-1.9.0/gallery_dl/cloudflare.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/config.py` & `gallery_dl-1.9.0/gallery_dl/config.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/downloader/__init__.py` & `gallery_dl-1.9.0/gallery_dl/downloader/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,22 +18,31 @@
 
 
 def find(scheme):
     """Return downloader class suitable for handling the given scheme"""
     try:
         return _cache[scheme]
     except KeyError:
-        klass = None
+        pass
+
+    klass = None
+    if scheme == "https":
+        scheme = "http"
+    if scheme in modules:  # prevent unwanted imports
         try:
-            if scheme in modules:  # prevent unwanted imports
-                module = importlib.import_module("." + scheme, __package__)
-                klass = module.__downloader__
-        except (ImportError, AttributeError, TypeError):
+            module = importlib.import_module("." + scheme, __package__)
+        except ImportError:
             pass
+        else:
+            klass = module.__downloader__
+
+    if scheme == "http":
+        _cache["http"] = _cache["https"] = klass
+    else:
         _cache[scheme] = klass
-        return klass
+    return klass
 
 
 # --------------------------------------------------------------------
 # internals
 
 _cache = {}
```

### Comparing `gallery_dl-1.8.7/gallery_dl/downloader/text.py` & `gallery_dl-1.9.0/gallery_dl/downloader/text.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,26 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2014-2018 Mike Fährmann
+# Copyright 2014-2019 Mike Fährmann
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License version 2 as
 # published by the Free Software Foundation.
 
 """Downloader module for text: URLs"""
 
 from .common import DownloaderBase
 
 
 class TextDownloader(DownloaderBase):
     scheme = "text"
 
-    def __init__(self, extractor, output):
-        DownloaderBase.__init__(self, extractor, output)
-        self.content = b""
-
-    def connect(self, url, offset):
-        data = url.encode()
-        self.content = data[offset + 5:]
-        return offset, len(data) - 5
-
-    def receive(self, file):
-        file.write(self.content)
-
-    def reset(self):
-        self.content = b""
-
-    @staticmethod
-    def get_extension():
-        return "txt"
+    def download(self, url, pathfmt):
+        if self.part:
+            pathfmt.part_enable(self.partdir)
+        self.out.start(pathfmt.path)
+        with pathfmt.open("wb") as file:
+            file.write(url.encode()[5:])
+        return True
 
 
 __downloader__ = TextDownloader
```

### Comparing `gallery_dl-1.8.7/gallery_dl/downloader/ytdl.py` & `gallery_dl-1.9.0/gallery_dl/downloader/ytdl.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,30 +16,35 @@
 
 class YoutubeDLDownloader(DownloaderBase):
     scheme = "ytdl"
 
     def __init__(self, extractor, output):
         DownloaderBase.__init__(self, extractor, output)
 
+        retries = self.config("retries", extractor._retries)
         options = {
             "format": self.config("format") or None,
             "ratelimit": text.parse_bytes(self.config("rate"), None),
-            "retries": self.config("retries", extractor._retries),
+            "retries": retries+1 if retries >= 0 else float("inf"),
             "socket_timeout": self.config("timeout", extractor._timeout),
             "nocheckcertificate": not self.config("verify", extractor._verify),
             "nopart": not self.part,
+            "updatetime": self.config("mtime", True),
         }
         options.update(self.config("raw-options") or {})
 
         if self.config("logging", True):
             options["logger"] = self.log
 
         self.ytdl = YoutubeDL(options)
 
     def download(self, url, pathfmt):
+        for cookie in self.session.cookies:
+            self.ytdl.cookiejar.set_cookie(cookie)
+
         try:
             info_dict = self.ytdl.extract_info(url[5:], download=False)
         except Exception:
             return False
 
         if "entries" in info_dict:
             index = pathfmt.keywords.get("_ytdl_index")
```

### Comparing `gallery_dl-1.8.7/gallery_dl/exception.py` & `gallery_dl-1.9.0/gallery_dl/exception.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/2chan.py` & `gallery_dl-1.9.0/gallery_dl/extractor/2chan.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/35photo.py` & `gallery_dl-1.9.0/gallery_dl/extractor/35photo.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,15 +68,14 @@
             "favorites"  : data["photo_fav"],
             "score"      : data["photo_rating"],
             "type"       : data["photo_type"],
             "date"       : data["timeAdd"],
             "user"       : data["user_login"],
             "user_id"    : data["user_id"],
             "user_name"  : data["user_name"],
-            "other"      : data["otherData"],
         }
 
         if "series" in data:
             for info["num"], photo in enumerate(data["series"], 1):
                 info["url"] = photo["src"]
                 info["id_series"] = text.parse_int(photo["id"])
                 info["title_series"] = photo["title"] or ""
@@ -85,26 +84,28 @@
             info["num"] = 1
             yield info
 
     @staticmethod
     def _photo_ids(page):
         """Extract unique photo IDs and return them as sorted list"""
         #  searching for photo-id="..." doesn't always work (see unit tests)
+        if not page:
+            return ()
         return sorted(
             set(text.extract_iter(page, "/photo_", "/")),
             key=text.parse_int,
             reverse=True,
         )
 
 
 class _35photoUserExtractor(_35photoExtractor):
     """Extractor for all images of a user on 35photo.pro"""
     subcategory = "user"
     pattern = (r"(?:https?://)?(?:[a-z]+\.)?35photo\.pro"
-               r"/(?!photo_|genre_)([^/?&#]+)")
+               r"/(?!photo_|genre_|rating/)([^/?&#]+)")
     test = (
         ("https://35photo.pro/liya", {
             "pattern": r"https://m\d+.35photo.pro/photos_(main|series)/.*.jpg",
             "count": 9,
         }),
         ("https://35photo.pro/suhoveev", {
             # last photo ID (1267028) isn't given as 'photo-id="<id>"
@@ -142,15 +143,22 @@
     directory_fmt = ("{category}", "Genre", "{genre}")
     archive_fmt = "g{genre_id}_{id}_{num}"
     pattern = r"(?:https?://)?(?:[a-z]+\.)?35photo\.pro/genre_(\d+)(/new/)?"
     test = (
         ("https://35photo.pro/genre_109/", {
             "range": "1-30",
         }),
-        ("https://35photo.pro/genre_109/new/"),
+        ("https://35photo.pro/genre_103/", {
+            "range": "1-30",
+            "count": 30,
+        }),
+        ("https://35photo.pro/genre_103/new/", {
+            "range": "1-30",
+            "count": 30,
+        }),
     )
 
     def __init__(self, match):
         _35photoExtractor.__init__(self, match)
         self.genre_id, self.new = match.groups()
         self.photo_ids = None
 
@@ -161,14 +169,16 @@
             page, ' class="photo', '\n')[0])
         return {
             "genre": text.extract(page, " genre - ", ". ")[0],
             "genre_id": text.parse_int(self.genre_id),
         }
 
     def photos(self):
+        if not self.photo_ids:
+            return ()
         return self._pagination({
             "page": "genre",
             "community_id": self.genre_id,
             "photo_rating": "0" if self.new else "50",
             "lastId": self.photo_ids[-1],
         }, self.photo_ids)
 
@@ -189,15 +199,14 @@
             "favorites"  : int,
             "score"      : int,
             "type"       : 0,
             "date"       : "15 авг, 2014",
             "user"       : "liya",
             "user_id"    : 20415,
             "user_name"  : "Liya Mirzaeva",
-            "other"      : str,
         },
     })
 
     def __init__(self, match):
         _35photoExtractor.__init__(self, match)
         self.photo_id = match.group(1)
```

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/3dbooru.py` & `gallery_dl-1.9.0/gallery_dl/extractor/3dbooru.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/4chan.py` & `gallery_dl-1.9.0/gallery_dl/extractor/4chan.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/500px.py` & `gallery_dl-1.9.0/gallery_dl/extractor/500px.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,16 +27,15 @@
     def items(self):
         first = True
         data = self.metadata()
         yield Message.Version, 1
 
         for photo in self.photos():
             url = photo["images"][-1]["url"]
-            fmt = photo["image_format"]
-            photo["extension"] = "jpg" if fmt == "jpeg" else fmt
+            photo["extension"] = photo["image_format"]
             if data:
                 photo.update(data)
             if first:
                 first = False
                 yield Message.Directory, photo
             yield Message.Url, url, photo
 
@@ -55,15 +54,15 @@
             "include_geo"           : "true",
             "include_equipment_info": "true",
             "vendor_photos"         : "true",
             "include_licensing"     : "true",
             "include_releases"      : "true",
             "liked_by"              : "1",
             "following_sample"      : "100",
-            "image_size"            : "32768",
+            "image_size"            : "4096",
             "ids"                   : ",".join(str(p["id"]) for p in photos),
         }
 
         data = self._api_call(url, params)["photos"]
         for photo in photos:
             pid = str(photo["id"])
             photo.update(data[pid])
@@ -86,15 +85,15 @@
 
 class _500pxUserExtractor(_500pxExtractor):
     """Extractor for photos from a user's photostream on 500px.com"""
     subcategory = "user"
     pattern = (r"(?:https?://)?500px\.com"
                r"/(?!photo/)([^/?&#]+)/?(?:$|\?|#)")
     test = ("https://500px.com/light_expression_photography", {
-        "pattern": r"https?://drscdn.500px.org/photo/\d+/m%3D5000/v2",
+        "pattern": r"https?://drscdn.500px.org/photo/\d+/m%3D4096/v2",
         "range": "1-99",
         "count": 99,
     })
 
     def __init__(self, match):
         _500pxExtractor.__init__(self, match)
         self.user = match.group(1)
@@ -120,15 +119,15 @@
 class _500pxGalleryExtractor(_500pxExtractor):
     """Extractor for photo galleries on 500px.com"""
     subcategory = "gallery"
     directory_fmt = ("{category}", "{user[username]}", "{gallery[name]}")
     pattern = (r"(?:https?://)?500px\.com"
                r"/(?!photo/)([^/?&#]+)/galleries/([^/?&#]+)")
     test = ("https://500px.com/fashvamp/galleries/lera", {
-        "url": "8a520272ece83278166b4f8556f9c9da43c43c45",
+        "url": "002dc81dee5b4a655f0e31ad8349e8903b296df6",
         "count": 3,
         "keyword": {
             "gallery": dict,
             "user": dict,
         },
     })
 
@@ -140,15 +139,15 @@
     def metadata(self):
         # get csrf token and user id from webpage
         url = "{}/{}/galleries/{}".format(
             self.root, self.user_name, self.gallery_name)
         page = self.request(url).text
         self.csrf_token, pos = text.extract(page, 'csrf-token" content="', '"')
         self.user_id   , pos = text.extract(page, 'App.CuratorId =', '\n', pos)
-        self.user_id = self.user_id.strip()
+        self.user_id = self.user_id.strip(" '\";")
 
         # get gallery metadata; transform gallery name into id
         url = "https://api.500px.com/v1/users/{}/galleries/{}".format(
             self.user_id, self.gallery_name)
         params = {
             #  "include_user": "true",
             "include_cover": "1",
@@ -170,61 +169,50 @@
 
 
 class _500pxImageExtractor(_500pxExtractor):
     """Extractor for individual images from 500px.com"""
     subcategory = "image"
     pattern = r"(?:https?://)?500px\.com/photo/(\d+)"
     test = ("https://500px.com/photo/222049255/queen-of-coasts", {
-        "url": "d1eda7afeaa589f71f05b9bb5c0694e3ffb357cd",
+        "url": "fbdf7df39325cae02f5688e9f92935b0e7113315",
         "count": 1,
         "keyword": {
             "camera": "Canon EOS 600D",
             "camera_info": dict,
-            "collections_count": int,
             "comments": list,
             "comments_count": int,
-            "converted": False,
-            "converted_bits": int,
-            "created_at": "2017-08-01T04:40:05-04:00",
-            "crop_version": 0,
+            "created_at": "2017-08-01T08:40:05+00:00",
             "description": str,
-            "editored_by": dict,
+            "editored_by": None,
             "editors_choice": False,
             "extension": "jpg",
-            "favorites_count": int,
             "feature": "popular",
             "feature_date": "2017-08-01T09:58:28+00:00",
             "focal_length": "208",
             "height": 3111,
             "id": 222049255,
-            "image_format": "jpeg",
-            "image_url": str,
+            "image_format": "jpg",
+            "image_url": list,
             "images": list,
             "iso": "100",
             "lens": "EF-S55-250mm f/4-5.6 IS II",
             "lens_info": dict,
-            "license_type": 0,
-            "licensed_at": None,
-            "liked": False,
+            "liked": None,
             "location": None,
             "location_details": dict,
             "name": "Queen Of Coasts",
             "nsfw": False,
             "privacy": False,
             "profile": True,
             "rating": float,
-            "sales_count": int,
             "status": 1,
-            "store_download": False,
-            "store_height": 3111,
-            "store_width": 4637,
             "tags": list,
-            "taken_at": "2017-05-04T13:36:51-04:00",
+            "taken_at": "2017-05-04T17:36:51+00:00",
             "times_viewed": int,
-            "url": "/photo/222049255/queen-of-coasts-by-olesya-nabieva",
+            "url": "/photo/222049255/Queen-Of-Coasts-by-Olesya-Nabieva",
             "user": dict,
             "user_id": 12847235,
             "votes_count": int,
             "watermark": True,
             "width": 4637,
         },
     })
```

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/8chan.py` & `gallery_dl-1.9.0/gallery_dl/extractor/8chan.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/8muses.py` & `gallery_dl-1.9.0/gallery_dl/extractor/8muses.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/__init__.py` & `gallery_dl-1.9.0/gallery_dl/extractor/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     "artstation",
     "behance",
     "bobx",
     "danbooru",
     "deviantart",
     "dynastyscans",
     "e621",
+    "erolord",
     "exhentai",
     "fallenangels",
     "flickr",
     "gelbooru",
     "gfycat",
     "hbrowse",
     "hentai2read",
```

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/artstation.py` & `gallery_dl-1.9.0/gallery_dl/extractor/artstation.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,17 +75,15 @@
             for asset in assets:
                 data["asset"] = asset
                 yield data.copy()
 
     def get_user_info(self, username):
         """Return metadata for a specific user"""
         url = "{}/users/{}/quick.json".format(self.root, username.lower())
-        response = self.request(url, expect=(404,))
-        if response.status_code == 404:
-            raise exception.NotFoundError("user")
+        response = self.request(url, notfound="user")
         return response.json()
 
     def _pagination(self, url, params=None):
         if not params:
             params = {}
         params["page"] = 1
         total = 0
```

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/behance.py` & `gallery_dl-1.9.0/gallery_dl/extractor/behance.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/bobx.py` & `gallery_dl-1.9.0/gallery_dl/extractor/bobx.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/booru.py` & `gallery_dl-1.9.0/gallery_dl/extractor/booru.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/chan.py` & `gallery_dl-1.9.0/gallery_dl/extractor/chan.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/common.py` & `gallery_dl-1.9.0/gallery_dl/extractor/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 """Common classes and constants used by extractor modules."""
 
 import re
 import time
 import netrc
 import queue
 import logging
+import datetime
 import requests
 import threading
 import http.cookiejar
 from .message import Message
 from .. import config, text, exception, cloudflare
 
 
@@ -35,18 +36,21 @@
     def __init__(self, match):
         self.session = requests.Session()
         self.log = logging.getLogger(self.category)
         self.url = match.string
         self._init_headers()
         self._init_cookies()
         self._init_proxies()
-        self._retries = self.config("retries", 5)
+        self._retries = self.config("retries", 4)
         self._timeout = self.config("timeout", 30)
         self._verify = self.config("verify", True)
 
+        if self._retries < 0:
+            self._retries = float("inf")
+
     @classmethod
     def from_url(cls, url):
         if isinstance(cls.pattern, str):
             cls.pattern = re.compile(cls.pattern)
         match = cls.pattern.match(url)
         return cls(match) if match else None
 
@@ -59,19 +63,19 @@
     def skip(self, num):
         return 0
 
     def config(self, key, default=None):
         return config.interpolate(
             ("extractor", self.category, self.subcategory, key), default)
 
-    def request(self, url, method="GET", *, session=None,
-                encoding=None, expect=(), retries=None, **kwargs):
-        tries = 0
-        retries = retries or self._retries
-        session = session or self.session
+    def request(self, url, method="GET", *, session=None, retries=None,
+                encoding=None, fatal=True, notfound=None, **kwargs):
+        tries = 1
+        retries = self._retries if retries is None else retries
+        session = self.session if session is None else session
         kwargs.setdefault("timeout", self._timeout)
         kwargs.setdefault("verify", self._verify)
 
         while True:
             try:
                 response = session.request(method, url, **kwargs)
             except (requests.exceptions.ConnectionError,
@@ -79,34 +83,45 @@
                     requests.exceptions.ChunkedEncodingError,
                     requests.exceptions.ContentDecodingError) as exc:
                 msg = exc
             except (requests.exceptions.RequestException) as exc:
                 raise exception.HttpError(exc)
             else:
                 code = response.status_code
-                if 200 <= code < 400 or code in expect:
+                if 200 <= code < 400 or not fatal and \
+                        (400 <= code < 429 or 431 <= code < 500):
                     if encoding:
                         response.encoding = encoding
                     return response
+                if notfound and code == 404:
+                    raise exception.NotFoundError(notfound)
                 if cloudflare.is_challenge(response):
                     self.log.info("Solving Cloudflare challenge")
                     url, domain, cookies = cloudflare.solve_challenge(
                         session, response, kwargs)
                     cloudflare.cookies.update(self.category, (domain, cookies))
                     continue
+                if cloudflare.is_captcha(response):
+                    try:
+                        import OpenSSL  # noqa
+                    except ImportError:
+                        msg = " - Install 'pyOpenSSL' and try again"
+                    else:
+                        msg = ""
+                    self.log.warning("Cloudflare CAPTCHA" + msg)
 
                 msg = "{}: {} for url: {}".format(code, response.reason, url)
-                if code < 500 and code != 429:
+                if code < 500 and code != 429 and code != 430:
                     break
 
-            tries += 1
-            self.log.debug("%s (%d/%d)", msg, tries, retries)
-            if tries >= retries:
+            self.log.debug("%s (%s/%s)", msg, tries, retries+1)
+            if tries > retries:
                 break
-            time.sleep(2 ** tries)
+            time.sleep(min(2 ** (tries-1), 1800))
+            tries += 1
 
         raise exception.HttpError(msg)
 
     def _get_auth_info(self):
         """Return authentication information as (username, password) tuple"""
         username = self.config("username")
         password = None
@@ -126,16 +141,16 @@
 
     def _init_headers(self):
         """Set additional headers for the 'session' object"""
         headers = self.session.headers
         headers.clear()
 
         headers["User-Agent"] = self.config(
-            "user-agent", ("Mozilla/5.0 (X11; Linux x86_64; rv:62.0) "
-                           "Gecko/20100101 Firefox/62.0"))
+            "user-agent", ("Mozilla/5.0 (X11; Linux x86_64; rv:68.0) "
+                           "Gecko/20100101 Firefox/68.0"))
         headers["Accept"] = "*/*"
         headers["Accept-Language"] = "en-US,en;q=0.5"
         headers["Accept-Encoding"] = "gzip, deflate"
         headers["Connection"] = "keep-alive"
         headers["Upgrade-Insecure-Requests"] = "1"
 
     def _init_proxies(self):
@@ -199,14 +214,28 @@
         try:
             for name in cookienames:
                 self.session.cookies._find(name, domain)
         except KeyError:
             return False
         return True
 
+    def _get_date_min_max(self, dmin=None, dmax=None):
+        """Retrieve and parse 'date-min' and 'date-max' config values"""
+        def get(key, default):
+            ts = self.config(key, default)
+            if isinstance(ts, str):
+                try:
+                    ts = int(datetime.datetime.strptime(ts, fmt).timestamp())
+                except ValueError as exc:
+                    self.log.warning("Unable to parse '%s': %s", key, exc)
+                    ts = default
+            return ts
+        fmt = self.config("date-format", "%Y-%m-%dT%H:%M:%S")
+        return get("date-min", dmin), get("date-max", dmax)
+
     @classmethod
     def _get_tests(cls):
         """Yield an extractor's test cases as (URL, RESULTS) tuples"""
         tests = cls.test
         if not tests:
             return
 
@@ -399,34 +428,40 @@
 
 
 # Reduce strictness of the expected magic string in cookiejar files.
 # (This allows the use of Wget-generated cookiejars without modification)
 http.cookiejar.MozillaCookieJar.magic_re = re.compile(
     "#( Netscape)? HTTP Cookie File", re.IGNORECASE)
 
-# Update default cipher list of urllib3
-# to fix issues with Cloudflare and, by extension, Artstation (#227)
-from requests.packages.urllib3.util import ssl_  # noqa
-logging.getLogger("gallery-dl").debug("updating default urllib3 ciphers")
-
-# cipher list taken from urllib3 1.25
-# https://github.com/urllib3/urllib3/blob/1.25/src/urllib3/util/ssl_.py
-# with additions from
-# https://github.com/Anorov/cloudflare-scrape/pull/242
-ssl_.DEFAULT_CIPHERS = (
-    "ECDHE+AESGCM:"
-    "ECDHE+CHACHA20:"
-    "DHE+AESGCM:"
-    "DHE+CHACHA20:"
-    "ECDH+AESGCM:"
-    "DH+AESGCM:"
-    "ECDH+AES:"
-    "DH+AES:"
-    "RSA+AESGCM:"
-    "RSA+AES:"
-    "!ECDHE+SHA:"
-    "!AES128-SHA:"
-    "!aNULL:"
-    "!eNULL:"
-    "!MD5:"
-    "!DSS"
-)
+# Replace default cipher list of urllib3 to avoid Cloudflare CAPTCHAs
+ciphers = config.get(("ciphers",), True)
+if ciphers:
+    logging.getLogger("gallery-dl").debug("Updating urllib3 ciphers")
+
+    if ciphers is True:
+        ciphers = (
+            # Firefox's list
+            "TLS_AES_128_GCM_SHA256:"
+            "TLS_CHACHA20_POLY1305_SHA256:"
+            "TLS_AES_256_GCM_SHA384:"
+            "ECDHE-ECDSA-AES128-GCM-SHA256:"
+            "ECDHE-RSA-AES128-GCM-SHA256:"
+            "ECDHE-ECDSA-CHACHA20-POLY1305:"
+            "ECDHE-RSA-CHACHA20-POLY1305:"
+            "ECDHE-ECDSA-AES256-GCM-SHA384:"
+            "ECDHE-RSA-AES256-GCM-SHA384:"
+            "ECDHE-ECDSA-AES256-SHA:"
+            "ECDHE-ECDSA-AES128-SHA:"
+            "ECDHE-RSA-AES128-SHA:"
+            "ECDHE-RSA-AES256-SHA:"
+            "DHE-RSA-AES128-SHA:"
+            "DHE-RSA-AES256-SHA:"
+            "AES128-SHA:"
+            "AES256-SHA:"
+            "DES-CBC3-SHA"
+        )
+    elif isinstance(ciphers, list):
+        ciphers = ":".join(ciphers)
+
+    from requests.packages.urllib3.util import ssl_  # noqa
+    ssl_.DEFAULT_CIPHERS = ciphers
+    del ssl_
```

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/danbooru.py` & `gallery_dl-1.9.0/gallery_dl/extractor/danbooru.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/deviantart.py` & `gallery_dl-1.9.0/gallery_dl/extractor/deviantart.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,16 +201,15 @@
         )
 
         deviation["extension"] = "txt"
         return Message.Url, txt, deviation
 
     @staticmethod
     def _find_folder(folders, name):
-        pattern = re.compile(
-            r"[^\w]*" + name.replace("-", r"[^\w]+") + r"[^\w]*$")
+        pattern = re.compile(r"(?i)\W*" + name.replace("-", r"\W+") + r"\W*$")
         for folder in folders:
             if pattern.match(folder["name"]):
                 return folder
         raise exception.NotFoundError("folder")
 
     def _folder_urls(self, folders, category):
         url = "{}/{}/{}/0/".format(self.root, self.user, category)
@@ -412,15 +411,15 @@
 
     def __init__(self, match):
         DeviantartExtractor.__init__(self, match)
         self.path = match.group(3)
 
     def deviations(self):
         url = "{}/{}/{}".format(self.root, self.user, self.path)
-        response = self._html_request(url, expect=range(400, 500))
+        response = self._html_request(url, fatal=False)
         deviation_id = text.extract(response.text, '//deviation/', '"')[0]
         if response.status_code >= 400 or not deviation_id:
             raise exception.NotFoundError("image")
         return (self.api.deviation(deviation_id),)
 
 
 class DeviantartStashExtractor(DeviantartExtractor):
@@ -763,15 +762,15 @@
                   "mature_content": self.mature}
         return self._pagination_folders(endpoint, params)
 
     @memcache(keyarg=1)
     def user_profile(self, username):
         """Get user profile information"""
         endpoint = "user/profile/" + username
-        return self._call(endpoint, expect_error=True)
+        return self._call(endpoint, fatal=False)
 
     def authenticate(self, refresh_token):
         """Authenticate the application by requesting an access token"""
         self.headers["Authorization"] = self._authenticate_impl(refresh_token)
 
     @cache(maxage=3600, keyarg=1)
     def _authenticate_impl(self, refresh_token):
@@ -793,36 +792,32 @@
         if response.status_code != 200:
             raise exception.AuthenticationError('"{} ({})"'.format(
                 data.get("error_description"), data.get("error")))
         if refresh_token:
             _refresh_token_cache.update(refresh_token, data["refresh_token"])
         return "Bearer " + data["access_token"]
 
-    def _call(self, endpoint, params=None, expect_error=False, public=True):
+    def _call(self, endpoint, params=None, fatal=True, public=True):
         """Call an API endpoint"""
         url = "https://www.deviantart.com/api/v1/oauth2/" + endpoint
         while True:
             if self.delay >= 0:
                 time.sleep(2 ** self.delay)
 
             self.authenticate(None if public else self.refresh_token)
             response = self.extractor.request(
-                url,
-                params=params,
-                headers=self.headers,
-                expect=range(400, 500),
-            )
+                url, headers=self.headers, params=params, fatal=False)
             data = response.json()
             status = response.status_code
 
             if 200 <= status < 400:
                 if self.delay > self.delay_min:
                     self.delay -= 1
                 return data
-            if expect_error:
+            if not fatal:
                 return None
             if data.get("error_description") == "User not found.":
                 raise exception.NotFoundError("user or group")
 
             self.log.debug(response.text)
             msg = "API responded with {} {}".format(
                 status, response.reason)
```

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/directlink.py` & `gallery_dl-1.9.0/gallery_dl/extractor/directlink.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/dynastyscans.py` & `gallery_dl-1.9.0/gallery_dl/extractor/dynastyscans.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/e621.py` & `gallery_dl-1.9.0/gallery_dl/extractor/e621.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/exhentai.py` & `gallery_dl-1.9.0/gallery_dl/extractor/exhentai.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,27 +255,27 @@
             yield url, text.nameext_from_url(imgurl, data)
 
             request["imgkey"] = nextkey
 
     def _gallery_page(self):
         url = "{}/g/{}/{}/".format(
             self.root, self.gallery_id, self.gallery_token)
-        response = self.request(url, expect=range(400, 500))
+        response = self.request(url, fatal=False)
         page = response.text
 
         if response.status_code == 404 and "Gallery Not Available" in page:
             raise exception.AuthorizationError()
         if page.startswith(("Key missing", "Gallery not found")):
             raise exception.NotFoundError("gallery")
         return page
 
     def _image_page(self):
         url = "{}/s/{}/{}-{}".format(
             self.root, self.image_token, self.gallery_id, self.image_num)
-        page = self.request(url, expect=range(400, 500)).text
+        page = self.request(url, fatal=False).text
 
         if page.startswith(("Invalid page", "Keep trying")):
             raise exception.NotFoundError("image page")
         return page
 
     def _check_limits(self, data):
         if not self._remaining or data["num"] % 20 == 0:
```

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/fallenangels.py` & `gallery_dl-1.9.0/gallery_dl/extractor/fallenangels.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/flickr.py` & `gallery_dl-1.9.0/gallery_dl/extractor/flickr.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/foolfuuka.py` & `gallery_dl-1.9.0/gallery_dl/extractor/foolfuuka.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/foolslide.py` & `gallery_dl-1.9.0/gallery_dl/extractor/foolslide.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/gelbooru.py` & `gallery_dl-1.9.0/gallery_dl/extractor/gelbooru.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/gfycat.py` & `gallery_dl-1.9.0/gallery_dl/extractor/gfycat.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/hbrowse.py` & `gallery_dl-1.9.0/gallery_dl/extractor/hbrowse.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/hentai2read.py` & `gallery_dl-1.9.0/gallery_dl/extractor/hentai2read.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/hentaicafe.py` & `gallery_dl-1.9.0/gallery_dl/extractor/hentaicafe.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/hentaifoundry.py` & `gallery_dl-1.9.0/gallery_dl/extractor/hentaifoundry.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/hentaifox.py` & `gallery_dl-1.9.0/gallery_dl/extractor/hentaifox.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/hentaihere.py` & `gallery_dl-1.9.0/gallery_dl/extractor/hentaihere.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/hentainexus.py` & `gallery_dl-1.9.0/gallery_dl/extractor/hentainexus.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/hitomi.py` & `gallery_dl-1.9.0/gallery_dl/extractor/hitomi.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/hypnohub.py` & `gallery_dl-1.9.0/gallery_dl/extractor/hypnohub.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/idolcomplex.py` & `gallery_dl-1.9.0/gallery_dl/extractor/idolcomplex.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/imagebam.py` & `gallery_dl-1.9.0/gallery_dl/extractor/imagebam.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/imagefap.py` & `gallery_dl-1.9.0/gallery_dl/extractor/imagefap.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/imagehosts.py` & `gallery_dl-1.9.0/gallery_dl/extractor/imagehosts.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/imgbox.py` & `gallery_dl-1.9.0/gallery_dl/extractor/imgbox.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/imgth.py` & `gallery_dl-1.9.0/gallery_dl/extractor/imgth.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/imgur.py` & `gallery_dl-1.9.0/gallery_dl/extractor/imgur.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,24 +12,23 @@
 from .. import text, exception
 import json
 
 
 class ImgurExtractor(Extractor):
     """Base class for imgur extractors"""
     category = "imgur"
+    root = "https://imgur.com"
 
     def __init__(self, match):
         Extractor.__init__(self, match)
         self.item_id = match.group(1)
         self.mp4 = self.config("mp4", True)
 
-    def _get_data(self, urlpart):
-        response = self.request("https://imgur.com/" + urlpart, expect=(404,))
-        if response.status_code == 404:
-            raise exception.NotFoundError(self.subcategory)
+    def _get_data(self, path):
+        response = self.request(self.root + path, notfound=self.subcategory)
         data = text.extract(response.text, "image               : ", ",\n")[0]
         return self._clean(json.loads(data))
 
     def _prepare(self, image):
         image["ext"] = image["ext"].partition("?")[0]
         if image["ext"] == ".gif" and (
                 (self.mp4 and image["prefer_video"]) or self.mp4 == "always"):
@@ -98,15 +97,15 @@
         ("https://i.imgur.com/21yMxCS.png"),  # direct link
         ("https://i.imgur.com/21yMxCSh.png"),  # direct link thumbnail
         ("https://i.imgur.com/zxaY6.gif"),  # direct link (short)
         ("https://i.imgur.com/zxaY6s.gif"),  # direct link (short; thumb)
     )
 
     def items(self):
-        image = self._get_data(self.item_id)
+        image = self._get_data("/" + self.item_id)
         url = self._prepare(image)
 
         yield Message.Version, 1
         yield Message.Directory, image
         yield Message.Url, url, image
 
 
@@ -161,21 +160,21 @@
             "exception": exception.NotFoundError,
         }),
         ("https://www.imgur.com/a/TcBmP"),  # www
         ("https://m.imgur.com/a/TcBmP"),  # mobile
     )
 
     def items(self):
-        album = self._get_data("a/" + self.item_id + "/all")
+        album = self._get_data("/a/" + self.item_id + "/all")
         images = album["album_images"]["images"]
         del album["album_images"]
 
         if int(album["num_images"]) > len(images):
-            url = ("https://imgur.com/ajaxalbums/getimages/" +
-                   self.item_id + "/hit.json")
+            url = "{}/ajaxalbums/getimages/{}/hit.json".format(
+                self.root, self.item_id)
             images = self.request(url).json()["data"]["images"]
 
         yield Message.Version, 1
         yield Message.Directory, {"album": album, "count": len(images)}
         for num, image in enumerate(images, 1):
             url = self._prepare(image)
             image["num"] = num
```

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/instagram.py` & `gallery_dl-1.9.0/gallery_dl/extractor/instagram.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,43 +7,87 @@
 # published by the Free Software Foundation.
 
 """Extract images from https://www.instagram.com/"""
 
 import hashlib
 import json
 from .common import Extractor, Message
-from .. import text
+from .. import text, exception
+from ..cache import cache
 
 
 class InstagramExtractor(Extractor):
     """Base class for instagram extractors"""
     category = "instagram"
     directory_fmt = ("{category}", "{username}")
     filename_fmt = "{sidecar_media_id:?/_/}{media_id}.{extension}"
     archive_fmt = "{media_id}"
     root = "https://www.instagram.com"
+    cookiedomain = ".instagram.com"
+    cookienames = ("sessionid",)
 
     def get_metadata(self):
         return {}
 
     def items(self):
+        self.login()
         yield Message.Version, 1
 
         metadata = self.get_metadata()
         for data in self.instagrams():
             data.update(metadata)
             yield Message.Directory, data
 
             if data['typename'] == 'GraphImage':
                 yield Message.Url, data['display_url'], \
                     text.nameext_from_url(data['display_url'], data)
             elif data['typename'] == 'GraphVideo':
                 yield Message.Url, \
                     'ytdl:{}/p/{}/'.format(self.root, data['shortcode']), data
 
+    def login(self):
+        if self._check_cookies(self.cookienames):
+            return
+        username, password = self._get_auth_info()
+        if username:
+            self.session.cookies.set("ig_cb", "1", domain="www.instagram.com")
+            self._update_cookies(self._login_impl(username, password))
+
+    @cache(maxage=360*24*3600, keyarg=1)
+    def _login_impl(self, username, password):
+        self.log.info("Logging in as %s", username)
+
+        page = self.request(self.root + "/accounts/login/").text
+        headers = {
+            "Referer"         : self.root + "/accounts/login/",
+            "X-IG-App-ID"     : "936619743392459",
+            "X-Requested-With": "XMLHttpRequest",
+        }
+
+        response = self.request(self.root + "/web/__mid/", headers=headers)
+        headers["X-CSRFToken"] = response.cookies["csrftoken"]
+        headers["X-Instagram-AJAX"] = text.extract(
+            page, '"rollout_hash":"', '"')[0]
+
+        url = self.root + "/accounts/login/ajax/"
+        data = {
+            "username"     : username,
+            "password"     : password,
+            "queryParams"  : "{}",
+            "optIntoOneTap": "true",
+        }
+        response = self.request(url, method="POST", headers=headers, data=data)
+
+        if not response.json().get("authenticated"):
+            raise exception.AuthenticationError()
+        return {
+            key: self.session.cookies.get(key)
+            for key in ("sessionid", "mid", "csrftoken")
+        }
+
     def _extract_shared_data(self, page):
         return json.loads(text.extract(page,
                           'window._sharedData = ', ';</script>')[0])
 
     def _extract_postpage(self, url):
         page = self.request(url).text
         shared_data = self._extract_shared_data(page)
```

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/keenspot.py` & `gallery_dl-1.9.0/gallery_dl/extractor/keenspot.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/khinsider.py` & `gallery_dl-1.9.0/gallery_dl/extractor/khinsider.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/kissmanga.py` & `gallery_dl-1.9.0/gallery_dl/extractor/kissmanga.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/komikcast.py` & `gallery_dl-1.9.0/gallery_dl/extractor/komikcast.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/konachan.py` & `gallery_dl-1.9.0/gallery_dl/extractor/konachan.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/livedoor.py` & `gallery_dl-1.9.0/gallery_dl/extractor/livedoor.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/luscious.py` & `gallery_dl-1.9.0/gallery_dl/extractor/luscious.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/mangadex.py` & `gallery_dl-1.9.0/gallery_dl/extractor/mangadex.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/mangafox.py` & `gallery_dl-1.9.0/gallery_dl/extractor/mangafox.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/mangahere.py` & `gallery_dl-1.9.0/gallery_dl/extractor/mangahere.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/mangapanda.py` & `gallery_dl-1.9.0/gallery_dl/extractor/mangapanda.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/mangapark.py` & `gallery_dl-1.9.0/gallery_dl/extractor/mangapark.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/mangareader.py` & `gallery_dl-1.9.0/gallery_dl/extractor/mangareader.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/mangastream.py` & `gallery_dl-1.9.0/gallery_dl/extractor/mangastream.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/mangoxo.py` & `gallery_dl-1.9.0/gallery_dl/extractor/mangoxo.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/mastodon.py` & `gallery_dl-1.9.0/gallery_dl/extractor/mastodon.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/message.py` & `gallery_dl-1.9.0/gallery_dl/extractor/message.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/myportfolio.py` & `gallery_dl-1.9.0/gallery_dl/extractor/myportfolio.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/newgrounds.py` & `gallery_dl-1.9.0/gallery_dl/extractor/newgrounds.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,30 +44,28 @@
         """Return urls of all relevant image pages"""
 
     def parse_page_data(self, page_url):
         """Collect url and metadata from an image page"""
         extr = text.extract_from(self.request(page_url).text)
         full = text.extract_from(json.loads(extr('"full_image_text":', '});')))
         data = {
+            "title"      : text.unescape(extr('"og:title" content="', '"')),
             "description": text.unescape(extr(':description" content="', '"')),
-            "date"       : extr('itemprop="datePublished" content="', '"'),
+            "date"       : text.parse_datetime(extr(
+                'itemprop="datePublished" content="', '"')),
             "rating"     : extr('class="rated-', '"'),
             "favorites"  : text.parse_int(extr('id="faves_load">', '<')),
             "score"      : text.parse_float(extr('id="score_number">', '<')),
+            "tags"       : text.split_html(extr(
+                '<dd class="tags momag">', '</dd>')),
             "url"        : full('src="', '"'),
-            "title"      : text.unescape(full('alt="', '"')),
             "width"      : text.parse_int(full('width="', '"')),
             "height"     : text.parse_int(full('height="', '"')),
         }
-
-        tags = text.split_html(extr('<dd class="tags momag">', '</dd>'))
-        tags.sort()
-        data["tags"] = tags
-
-        data["date"] = text.parse_datetime(data["date"])
+        data["tags"].sort()
         data["index"] = text.parse_int(
             data["url"].rpartition("/")[2].partition("_")[0])
         return data
 
     def _pagination(self, url):
         headers = {
             "Referer": self.root,
@@ -91,15 +89,15 @@
 class NewgroundsUserExtractor(NewgroundsExtractor):
     """Extractor for all images of a newgrounds user"""
     subcategory = "user"
     pattern = r"(?:https?://)?([^.]+)\.newgrounds\.com(?:/art)?/?$"
     test = (
         ("https://blitzwuff.newgrounds.com/art", {
             "url": "24b19c4a135a09889fac7b46a74e427e4308d02b",
-            "keyword": "2aab0532a894ff3cf88dd01ce5c60f114011b268",
+            "keyword": "98566e0c8096a8099b8d71962fea7e31c8b098d4",
         }),
         ("https://blitzwuff.newgrounds.com/"),
     )
 
     def get_page_urls(self):
         return self._pagination(self.root + "/art/page/1")
 
@@ -136,17 +134,17 @@
 
 
 class NewgroundsVideoExtractor(NewgroundsExtractor):
     """Extractor for all videos of a newgrounds user"""
     subcategory = "video"
     filename_fmt = "{category}_{index}.{extension}"
     pattern = r"(?:https?://)?([^.]+)\.newgrounds\.com/movies/?$"
-    test = ("https://twistedgrim.newgrounds.com/movies", {
+    test = ("https://tomfulp.newgrounds.com/movies", {
         "pattern": r"ytdl:https?://www\.newgrounds\.com/portal/view/\d+",
-        "count": ">= 29",
+        "count": ">= 32",
     })
 
     def get_page_urls(self):
         return self._pagination(self.root + "/movies/page/1")
 
     def parse_page_data(self, page_url):
         return {
```

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/ngomik.py` & `gallery_dl-1.9.0/gallery_dl/extractor/ngomik.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/nhentai.py` & `gallery_dl-1.9.0/gallery_dl/extractor/nhentai.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/nijie.py` & `gallery_dl-1.9.0/gallery_dl/extractor/nijie.py`

 * *Files 6% similar despite different names*

```diff
@@ -102,35 +102,30 @@
         return self.session.cookies
 
     def _pagination(self, path):
         url = "{}/{}.php".format(self.root, path)
         params = {"id": self.user_id, "p": 1}
 
         while True:
-            response = self.request(url, params=params, expect=(404,))
-            if response.status_code == 404:
-                raise exception.NotFoundError("artist")
-
-            page = response.text
-            ids = list(text.extract_iter(page, ' illust_id="', '"'))
-            yield from ids
+            page = self.request(url, params=params, notfound="artist").text
+            yield from text.extract_iter(page, 'illust_id="', '"')
 
             if '<a rel="next"' not in page:
                 return
             params["p"] += 1
 
 
 class NijieUserExtractor(NijieExtractor):
     """Extractor for works of a nijie-user"""
     subcategory = "user"
     pattern = (r"(?:https?://)?(?:www\.)?nijie\.info"
                r"/members(?:_illust)?\.php\?id=(\d+)")
     test = (
         ("https://nijie.info/members_illust.php?id=44", {
-            "url": "585d821df4716b1098660a0be426d01db4b65f2a",
+            "url": "66c4ff94c6e77c0765dd88f2d8c663055fda573e",
             "keyword": "d629c69e3172db1d7e026145e8eb640ac31ac16a",
         }),
         ("https://nijie.info/members_illust.php?id=43", {
             "exception": exception.NotFoundError,
         }),
         ("https://nijie.info/members.php?id=44"),
     )
@@ -170,15 +165,15 @@
 class NijieImageExtractor(NijieExtractor):
     """Extractor for a work/image from nijie.info"""
     subcategory = "image"
     pattern = (r"(?:https?://)?(?:www\.)?nijie\.info"
                r"/view(?:_popup)?\.php\?id=(\d+)")
     test = (
         ("https://nijie.info/view.php?id=70720", {
-            "url": "a10d4995645b5f260821e32c60a35f73546c2699",
+            "url": "5497f897311397dafa188521258624346a0af2a3",
             "keyword": "408393d010307c76d52cbd0a4368d6d357805aea",
             "content": "d85e3ea896ed5e4da0bca2390ad310a4df716ca6",
         }),
         ("https://nijie.info/view.php?id=70724", {
             "exception": exception.NotFoundError,
         }),
         ("https://nijie.info/view_popup.php?id=70720"),
@@ -186,18 +181,16 @@
 
     def __init__(self, match):
         NijieExtractor.__init__(self, match)
         self.image_id = match.group(1)
         self.page = ""
 
     def get_job_metadata(self):
-        response = self.request(self.view_url + self.image_id, expect=(404,))
-        if response.status_code == 404:
-            raise exception.NotFoundError("image")
-        self.page = response.text
+        self.page = self.request(
+            self.view_url + self.image_id, notfound="image").text
         self.user_id = text.extract(
             self.page, '"sameAs": "https://nijie.info/members.php?id=', '"')[0]
         return NijieExtractor.get_job_metadata(self)
 
     def get_image_ids(self):
         return (self.image_id,)
```

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/nsfwalbum.py` & `gallery_dl-1.9.0/gallery_dl/extractor/nsfwalbum.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/oauth.py` & `gallery_dl-1.9.0/gallery_dl/extractor/oauth.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/paheal.py` & `gallery_dl-1.9.0/gallery_dl/extractor/paheal.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/patreon.py` & `gallery_dl-1.9.0/gallery_dl/extractor/patreon.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/photobucket.py` & `gallery_dl-1.9.0/gallery_dl/extractor/photobucket.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/piczel.py` & `gallery_dl-1.9.0/gallery_dl/extractor/piczel.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/pinterest.py` & `gallery_dl-1.9.0/gallery_dl/extractor/pinterest.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,22 +224,22 @@
         return self._pagination("BoardRelatedPixieFeed", options)
 
     def _call(self, resource, options):
         url = "{}/resource/{}Resource/get/".format(self.BASE_URL, resource)
         params = {"data": json.dumps({"options": options}), "source_url": ""}
 
         response = self.extractor.request(
-            url, params=params, headers=self.HEADERS, expect=range(400, 500))
+            url, params=params, headers=self.HEADERS, fatal=False)
 
         try:
             data = response.json()
         except ValueError:
             data = {}
 
-        if 200 <= response.status_code < 400 and not response.history:
+        if response.status_code < 400 and not response.history:
             return data
 
         if response.status_code == 404 or response.history:
             resource = self.extractor.subcategory.rpartition("-")[2]
             raise exception.NotFoundError(resource)
         self.extractor.log.error("API request failed")
         self.extractor.log.debug("%s", response.text)
```

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/pixiv.py` & `gallery_dl-1.9.0/gallery_dl/extractor/pixiv.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,17 +139,15 @@
     def __init__(self, match):
         PixivExtractor.__init__(self, match)
         self.account = match.group(1)
 
     def items(self):
         url = "https://pixiv.me/" + self.account
         response = self.request(
-            url, method="HEAD", allow_redirects=False, expect=(404,))
-        if response.status_code == 404:
-            raise exception.NotFoundError("user")
+            url, method="HEAD", allow_redirects=False, notfound="user")
         yield Message.Version, 1
         yield Message.Queue, response.headers["Location"], {}
 
 
 class PixivWorkExtractor(PixivExtractor):
     """Extractor for a single pixiv work/illustration"""
     subcategory = "work"
@@ -441,15 +439,15 @@
         else:
             self.log.info("Logging in as %s", username)
             data["grant_type"] = "password"
             data["username"] = username
             data["password"] = password
 
         response = self.extractor.request(
-            url, method="POST", data=data, expect=(400,))
+            url, method="POST", data=data, fatal=False)
         if response.status_code >= 400:
             raise exception.AuthenticationError()
 
         data = response.json()["response"]
         if not refresh_token:
             _refresh_token_cache.update(username, data["refresh_token"])
         return data["user"], "Bearer " + data["access_token"]
@@ -487,18 +485,17 @@
         params = {"illust_id": illust_id}
         return self._call("v1/ugoira/metadata", params)["ugoira_metadata"]
 
     def _call(self, endpoint, params=None):
         url = "https://app-api.pixiv.net/" + endpoint
 
         self.login()
-        response = self.extractor.request(
-            url, params=params, expect=range(400, 500))
+        response = self.extractor.request(url, params=params, fatal=False)
 
-        if 200 <= response.status_code < 400:
+        if response.status_code < 400:
             return response.json()
         if response.status_code == 404:
             raise exception.NotFoundError()
         self.log.error("API request failed: %s", response.text)
         raise exception.StopExtraction()
 
     def _pagination(self, endpoint, params):
```

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/pixnet.py` & `gallery_dl-1.9.0/gallery_dl/extractor/pixnet.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/plurk.py` & `gallery_dl-1.9.0/gallery_dl/extractor/plurk.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/pornhub.py` & `gallery_dl-1.9.0/gallery_dl/extractor/pornhub.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/pururin.py` & `gallery_dl-1.9.0/gallery_dl/extractor/pururin.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/reactor.py` & `gallery_dl-1.9.0/gallery_dl/extractor/reactor.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/readcomiconline.py` & `gallery_dl-1.9.0/gallery_dl/extractor/readcomiconline.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/recursive.py` & `gallery_dl-1.9.0/gallery_dl/extractor/recursive.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/reddit.py` & `gallery_dl-1.9.0/gallery_dl/extractor/reddit.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 # published by the Free Software Foundation.
 
 """Extract images from subreddits at https://www.reddit.com/"""
 
 from .common import Extractor, Message
 from .. import text, util, extractor, exception
 from ..cache import cache
-import datetime
 import time
 
 
 class RedditExtractor(Extractor):
     """Base class for reddit extractors"""
     category = "reddit"
 
@@ -231,16 +230,15 @@
                 response.json().get("message"), response.status_code))
         return "Bearer " + response.json()["access_token"]
 
     def _call(self, endpoint, params):
         url = "https://oauth.reddit.com" + endpoint
         params["raw_json"] = 1
         self.authenticate()
-        response = self.extractor.request(
-            url, params=params, expect=range(400, 500))
+        response = self.extractor.request(url, params=params, fatal=False)
         remaining = response.headers.get("x-ratelimit-remaining")
         if remaining and float(remaining) < 2:
             wait = int(response.headers["x-ratelimit-reset"])
             self.log.info("Waiting %d seconds for ratelimit reset", wait)
             time.sleep(wait)
         data = response.json()
         if "error" in data:
@@ -248,20 +246,17 @@
                 raise exception.AuthorizationError()
             if data["error"] == 404:
                 raise exception.NotFoundError()
             raise Exception(data["message"])
         return data
 
     def _pagination(self, endpoint, params, _empty=()):
-        date_fmt = self.extractor.config("date-format", "%Y-%m-%dT%H:%M:%S")
-        date_min = self._parse_datetime("date-min", 0, date_fmt)
-        date_max = self._parse_datetime("date-max", 253402210800, date_fmt)
-
         id_min = self._parse_id("id-min", 0)
         id_max = self._parse_id("id-max", 2147483647)
+        date_min, date_max = self.extractor._get_date_min_max(0, 253402210800)
 
         while True:
             data = self._call(endpoint, params)["data"]
 
             for submission in data["children"]:
                 submission = submission["data"]
                 if (date_min <= submission["created_utc"] <= date_max and
@@ -290,24 +285,14 @@
             comment = comment["data"]
             yield comment
             if comment["replies"]:
                 queue += comment["replies"]["data"]["children"]
         if link_id and extra:
             yield from self.morechildren(link_id, extra)
 
-    def _parse_datetime(self, key, default, fmt):
-        ts = self.extractor.config(key, default)
-        if isinstance(ts, str):
-            try:
-                ts = int(datetime.datetime.strptime(ts, fmt).timestamp())
-            except ValueError as exc:
-                self.log.warning("Unable to parse '%s': %s", key, exc)
-                ts = default
-        return ts
-
     def _parse_id(self, key, default):
         sid = self.extractor.config(key)
         return self._decode(sid.rpartition("_")[2].lower()) if sid else default
 
     @staticmethod
     def _decode(sid):
         return util.bdecode(sid, "0123456789abcdefghijklmnopqrstuvwxyz")
```

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/rule34.py` & `gallery_dl-1.9.0/gallery_dl/extractor/rule34.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/safebooru.py` & `gallery_dl-1.9.0/gallery_dl/extractor/safebooru.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/sankaku.py` & `gallery_dl-1.9.0/gallery_dl/extractor/sankaku.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/sankakucomplex.py` & `gallery_dl-1.9.0/gallery_dl/extractor/sankakucomplex.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         pnum = 1
         last = None
         data = {"_extractor": SankakucomplexArticleExtractor}
 
         yield Message.Version, 1
         while True:
             url = "{}/{}/page/{}/".format(self.root, self.path, pnum)
-            response = self.request(url, expect=(404,))
-            if response.status_code == 404:
+            response = self.request(url, fatal=False)
+            if response.status_code >= 400:
                 return
             for url in text.extract_iter(response.text, 'data-direct="', '"'):
                 if url != last:
                     last = url
                     yield Message.Queue, url, data
             pnum += 1
```

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/seiga.py` & `gallery_dl-1.9.0/gallery_dl/extractor/seiga.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,17 +39,15 @@
     def get_images(self):
         """Return iterable containing metadata and images"""
 
     def get_image_url(self, image_id):
         """Get url for an image with id 'image_id'"""
         url = "{}/image/source/{}".format(self.root, image_id)
         response = self.request(
-            url, method="HEAD", allow_redirects=False, expect=(404,))
-        if response.status_code == 404:
-            raise exception.NotFoundError("image")
+            url, method="HEAD", allow_redirects=False, notfound="image")
         return response.headers["Location"].replace("/o/", "/priv/", 1)
 
     def login(self):
         """Login and set necessary cookies"""
         if not self._check_cookies(("user_session",)):
             username, password = self._get_auth_info()
             self._update_cookies(self._login_impl(username, password))
```

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/senmanga.py` & `gallery_dl-1.9.0/gallery_dl/extractor/senmanga.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/sexcom.py` & `gallery_dl-1.9.0/gallery_dl/extractor/sexcom.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,17 +19,17 @@
     filename_fmt = "{pin_id}{title:? //}.{extension}"
     archive_fmt = "{pin_id}"
     root = "https://www.sex.com"
 
     def items(self):
         yield Message.Version, 1
         yield Message.Directory, self.metadata()
-        for url in self.pins():
-            pin = self._parse_pin(url)
-            yield Message.Url, pin["url"], pin
+        for pin in map(self._parse_pin, self.pins()):
+            if pin:
+                yield Message.Url, pin["url"], pin
 
     def metadata(self):
         return {}
 
     def pins(self):
         return ()
 
@@ -45,16 +45,21 @@
 
             pager = extr('id="pagenum"', '</div>')
             url = text.extract(pager, ' href="', '"')[0]
             if not url:
                 return
             url = text.urljoin(self.root, url)
 
-    def _parse_pin(self, pin_url):
-        extr = text.extract_from(self.request(pin_url).text)
+    def _parse_pin(self, url):
+        response = self.request(url, fatal=False)
+        if response.status_code >= 400:
+            self.log.warning('Unable to fetch %s ("%s: %s")',
+                             url, response.status_code, response.reason)
+            return None
+        extr = text.extract_from(response.text)
         data = {}
 
         data["thumbnail"] = extr('itemprop="thumbnail" content="', '"')
         data["type"] = extr('<h1>' , '<').rstrip(" -").strip().lower()
         data["title"] = text.unescape(extr('itemprop="name">' , '<'))
         data["repins"] = text.parse_int(text.extract(
             extr('"btn-group"', '</div>'), '"btn btn-primary">' , '<')[0])
@@ -84,18 +89,18 @@
         data["tags"] = text.split_html(extr('class="tags"> Tags', '</div>'))
         data["comments"] = text.parse_int(extr('Comments (', ')'))
 
         return data
 
 
 class SexcomPinExtractor(SexcomExtractor):
-    """Extractor a pinned image or video on www.sex.com"""
+    """Extractor for a pinned image or video on www.sex.com"""
     subcategory = "pin"
     directory_fmt = ("{category}",)
-    pattern = r"(?:https?://)?(?:www\.)?sex\.com/pin/(\d+)"
+    pattern = r"(?:https?://)?(?:www\.)?sex\.com/pin/(\d+)(?!.*#related$)"
     test = (
         # picture
         ("https://www.sex.com/pin/56714360/", {
             "url": "599190d6e3d79f9f49dda194a0a58cb0ffa3ab86",
             "keyword": {
                 "comments": int,
                 "date": "2018-10-02T21:18:17-04:00",
@@ -120,24 +125,47 @@
         ("https://www.sex.com/pin/55748381/", {
             "pattern": "https://www.sex.com/video/stream/776238/hd",
         }),
         # pornhub embed
         ("https://www.sex.com/pin/55847384-very-nicely-animated/", {
             "pattern": "ytdl:https://www.pornhub.com/embed/ph56ef24b6750f2",
         }),
+        # 404
+        ("https://www.sex.com/pin/55847385/", {
+            "count": 0,
+        }),
     )
 
     def __init__(self, match):
         SexcomExtractor.__init__(self, match)
         self.pin_id = match.group(1)
 
     def pins(self):
         return ("{}/pin/{}/".format(self.root, self.pin_id),)
 
 
+class SexcomRelatedPinExtractor(SexcomPinExtractor):
+    """Extractor for related pins on www.sex.com"""
+    subcategory = "related-pin"
+    directory_fmt = ("{category}", "related {original_pin[pin_id]}")
+    pattern = r"(?:https?://)?(?:www\.)?sex\.com/pin/(\d+).*#related$"
+    test = ("https://www.sex.com/pin/56714360/#related", {
+        "count": 24,
+    })
+
+    def metadata(self):
+        pin = self._parse_pin(SexcomPinExtractor.pins(self)[0])
+        return {"original_pin": pin}
+
+    def pins(self):
+        url = "{}/pin/related?pinId={}&limit=24&offset=0".format(
+            self.root, self.pin_id)
+        return self._pagination(url)
+
+
 class SexcomBoardExtractor(SexcomExtractor):
     """Extractor for pins from a board on www.sex.com"""
     subcategory = "board"
     directory_fmt = ("{category}", "{user}", "{board}")
     pattern = (r"(?:https?://)?(?:www\.)?sex\.com/user"
                r"/([^/?&#]+)/(?!(?:following|pins|repins|likes)/)([^/?&#]+)")
     test = ("https://www.sex.com/user/ronin17/exciting-hentai/", {
```

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/shopify.py` & `gallery_dl-1.9.0/gallery_dl/extractor/shopify.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,52 +6,42 @@
 # it under the terms of the GNU General Public License version 2 as
 # published by the Free Software Foundation.
 
 """Extractors for Shopify instances"""
 
 from .common import Extractor, Message, SharedConfigMixin, generate_extractors
 from .. import text
-import time
 import re
 
 
 class ShopifyExtractor(SharedConfigMixin, Extractor):
     """Base class for Shopify extractors"""
     basecategory = "shopify"
     filename_fmt = "{product[title]}_{num:>02}_{id}.{extension}"
     archive_fmt = "{id}"
 
     def __init__(self, match):
         Extractor.__init__(self, match)
         self.item_url = self.root + match.group(1)
 
-    def request(self, url, method="GET", expect=range(400, 500), **kwargs):
-        tries = 0
-        kwargs["expect"] = expect
-        while True:
-            response = Extractor.request(self, url, method, **kwargs)
-            if response.status_code not in (429, 430):
-                return response
-            tries += 1
-            waittime = 2 ** (tries + 2)
-            self.log.warning(
-                "HTTP status %s: %s - Waiting for %d seconds",
-                response.status_code, response.reason, waittime)
-            time.sleep(waittime)
+    def request(self, url, **kwargs):
+        kwargs["retries"] = float("inf")
+        return Extractor.request(self, url, **kwargs)
 
     def items(self):
         data = self.metadata()
         yield Message.Version, 1
         yield Message.Directory, data
 
         headers = {"X-Requested-With": "XMLHttpRequest"}
         for url in self.products():
-            response = self.request(url + ".json", headers=headers)
+            response = self.request(
+                url + ".json", headers=headers, fatal=False)
             if response.status_code >= 400:
-                self.log.warning('Skipping %s ("%d: %s")',
+                self.log.warning('Skipping %s ("%s: %s")',
                                  url, response.status_code, response.reason)
                 continue
             product = response.json()["product"]
             del product["image"]
 
             for num, image in enumerate(product.pop("images"), 1):
                 text.nameext_from_url(image["src"], image)
@@ -85,18 +75,22 @@
         params = text.parse_query(self.params)
         params["page"] = text.parse_int(params.get("page"), 1)
         search_re = re.compile(r"/collections/[\w-]+/products/[\w-]+")
 
         while True:
             page = self.request(self.item_url, params=params).text
             urls = search_re.findall(page)
+            last = None
 
             if not urls:
                 return
             for path in urls:
+                if last == path:
+                    continue
+                last = path
                 yield self.root + path
             params["page"] += 1
 
 
 class ShopifyProductExtractor(ShopifyExtractor):
     """Base class for product extractors for Shopify based sites"""
     subcategory = "product"
@@ -109,15 +103,15 @@
 
 EXTRACTORS = {
     "fashionnova": {
         "root": "https://www.fashionnova.com",
         "pattern": r"(?:www\.)?fashionnova\.com",
         "test-product": (
             ("https://www.fashionnova.com/products/essential-slide-red", {
-                "pattern": r"https?://cdn\.shopify.com/",
+                "pattern": r"https?://cdn\d*\.shopify.com/",
                 "count": 3,
             }),
             ("https://www.fashionnova.com/collections/flats/products/name"),
         ),
         "test-collection": (
             ("https://www.fashionnova.com/collections/mini-dresses", {
                 "range": "1-20",
```

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/simplyhentai.py` & `gallery_dl-1.9.0/gallery_dl/extractor/simplyhentai.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     pattern = (r"(?:https?://)?(?!videos\.)([\w-]+\.simply-hentai\.com"
                r"(?!/(?:album|gifs?|images?|series)(?:/|$))"
                r"(?:/(?!(?:page|all-pages)(?:/|\.|$))[^/?&#]+)+)")
     test = (
         (("https://original-work.simply-hentai.com"
           "/amazon-no-hiyaku-amazon-elixir"), {
             "url": "258289249990502c3138719cb89e995a60861e49",
-            "keyword": "18ab9defca53dbb2aeb7965193e93e0ea125b76b",
+            "keyword": "eba83ccdbab3022a2280c77aa747f9458196138b",
         }),
         ("https://www.simply-hentai.com/notfound", {
             "exception": exception.GalleryDLException,
         }),
         # custom subdomain
         ("https://pokemon.simply-hentai.com/mao-friends-9bc39"),
         # www subdomain, two path segments
@@ -36,38 +36,34 @@
 
     def __init__(self, match):
         url = "https://" + match.group(1)
         GalleryExtractor.__init__(self, match, url)
         self.session.headers["Referer"] = url
 
     def metadata(self, page):
-        extr = text.extract
-        title , pos = extr(page, '<meta property="og:title" content="', '"')
+        extr = text.extract_from(page)
+        split = text.split_html
+
+        title = extr('<meta property="og:title" content="', '"')
         if not title:
             raise exception.NotFoundError("gallery")
-        gid   , pos = extr(page, '/Album/', '/', pos)
-        series, pos = extr(page, 'box-title">Series</div>', '</div>', pos)
-        lang  , pos = extr(page, 'box-title">Language</div>', '</div>', pos)
-        chars , pos = extr(page, 'box-title">Characters</div>', '</div>', pos)
-        tags  , pos = extr(page, 'box-title">Tags</div>', '</div>', pos)
-        artist, pos = extr(page, 'box-title">Artists</div>', '</div>', pos)
-        date  , pos = extr(page, 'Uploaded', '</div>', pos)
-        lang = text.remove_html(lang) if lang else None
-
-        return {
-            "gallery_id": text.parse_int(gid),
+        data = {
             "title"     : text.unescape(title),
-            "artist"    : text.split_html(artist),
-            "parody"    : text.split_html(series),
-            "characters": text.split_html(chars),
-            "tags"      : text.split_html(tags),
-            "lang"      : util.language_to_code(lang),
-            "language"  : lang,
-            "date"      : text.remove_html(date),
+            "gallery_id": text.parse_int(extr('/Album/', '/')),
+            "parody"    : split(extr('box-title">Series</div>', '</div>')),
+            "language"  : text.remove_html(extr(
+                'box-title">Language</div>', '</div>')) or None,
+            "characters": split(extr('box-title">Characters</div>', '</div>')),
+            "tags"      : split(extr('box-title">Tags</div>', '</div>')),
+            "artist"    : split(extr('box-title">Artists</div>', '</div>')),
+            "date"      : text.parse_datetime(text.remove_html(
+                extr('Uploaded', '</div>')), "%d.%m.%Y"),
         }
+        data["lang"] = util.language_to_code(data["language"])
+        return data
 
     def images(self, _):
         url = self.chapter_url + "/all-pages"
         headers = {"Accept": "application/json"}
         images = self.request(url, headers=headers).json()
         return [
             (urls["full"], {"image_id": text.parse_int(image_id)})
@@ -98,20 +94,19 @@
 
     def __init__(self, match):
         Extractor.__init__(self, match)
         self.page_url = "https://www." + match.group(1)
         self.type = match.group(2)
 
     def items(self):
-        page = self.request(self.page_url).text
-        url_search = 'data-src="' if self.type == "image" else '<source src="'
-
-        title, pos = text.extract(page, '"og:title" content="', '"')
-        descr, pos = text.extract(page, '"og:description" content="', '"', pos)
-        url  , pos = text.extract(page, url_search, '"', pos)
+        extr = text.extract_from(self.request(self.page_url).text)
+        title = extr('"og:title" content="'      , '"')
+        descr = extr('"og:description" content="', '"')
+        url = extr('&quot;image&quot;:&quot;'  , '&')
+        url = extr("&quot;content&quot;:&quot;", "&") or url
 
         tags = text.extract(descr, " tagged with ", " online for free ")[0]
         if tags:
             tags = tags.split(", ")
             tags[-1] = tags[-1].partition(" ")[2]
         else:
             tags = []
@@ -136,21 +131,21 @@
     filename_fmt = "{title}{episode:?_//>02}.{extension}"
     archive_fmt = "{title}_{episode}"
     pattern = r"(?:https?://)?(videos\.simply-hentai\.com/[^/?&#]+)"
     test = (
         ("https://videos.simply-hentai.com/creamy-pie-episode-02", {
             "pattern": r"https://www\.googleapis\.com/drive/v3/files"
                        r"/0B1ecQ8ZVLm3JcHZzQzBnVy1ZUmc\?alt=media&key=[\w-]+",
-            "keyword": "29d63987fed33f0a9f4b3786d1d71b03d793250a",
+            "keyword": "706790708b14773efc1e075ddd3b738a375348a5",
             "count": 1,
         }),
         (("https://videos.simply-hentai.com"
           "/1715-tifa-in-hentai-gang-bang-3d-movie"), {
             "url": "ad9a36ae06c601b6490e3c401834b4949d947eb0",
-            "keyword": "c561341aa3c6999f615abf1971d28fb2a83da2a7",
+            "keyword": "f9dad94fbde9c95859e631ff4f07297a9567b874",
         }),
     )
 
     def __init__(self, match):
         Extractor.__init__(self, match)
         self.page_url = "https://" + match.group(1)
 
@@ -174,14 +169,15 @@
             video_url = text.extract(embed_page, '"file":"', '"')[0]
             title, _, episode = title.rpartition(" Episode ")
 
         data = text.nameext_from_url(video_url, {
             "title": text.unescape(title),
             "episode": text.parse_int(episode),
             "tags": text.split_html(tags)[::2],
-            "date": text.remove_html(date),
             "type": "video",
+            "date": text.parse_datetime(text.remove_html(
+                date), "%B %d, %Y %H:%M"),
         })
 
         yield Message.Version, 1
         yield Message.Directory, data
         yield Message.Url, video_url, data
```

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/slickpic.py` & `gallery_dl-1.9.0/gallery_dl/extractor/slickpic.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/slideshare.py` & `gallery_dl-1.9.0/gallery_dl/extractor/slideshare.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/smugmug.py` & `gallery_dl-1.9.0/gallery_dl/extractor/smugmug.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,19 +65,19 @@
 class SmugmugAlbumExtractor(SmugmugExtractor):
     """Extractor for smugmug albums"""
     subcategory = "album"
     directory_fmt = ("{category}", "{User[NickName]}", "{Album[Name]}")
     archive_fmt = "a_{Album[AlbumKey]}_{Image[ImageKey]}"
     pattern = r"smugmug:album:([^:]+)$"
     test = (
-        ("smugmug:album:ddvxpg", {
-            "url": "0429e9bf50ee600674e448934e3882ca1761ae7b",
+        ("smugmug:album:cr4C7f", {
+            "url": "1436ee98d5797b308ecce5862e4885944f59c03c",
         }),
         # empty
-        ("smugmug:album:SXvjbW", {
+        ("smugmug:album:Fb7hMs", {
             "count": 0,
         }),
         # no "User"
         ("smugmug:album:6VRT8G", {
             "url": "c4a0f4c4bfd514b93cbdeb02b3345bf7ef6604df",
         }),
     )
@@ -105,18 +105,18 @@
 
 class SmugmugImageExtractor(SmugmugExtractor):
     """Extractor for individual smugmug images"""
     subcategory = "image"
     archive_fmt = "{Image[ImageKey]}"
     pattern = BASE_PATTERN + r"(?:/[^/?&#]+)+/i-([^/?&#-]+)"
     test = (
-        ("https://acapella.smugmug.com/Micro-Macro/Drops/i-g2Dmf9z", {
-            "url": "78f0bf3516b6d670b7319216bdeccb35942ca4cf",
-            "keyword": "b298ef7ed2b1918263b6a7dc6f56e54401584381",
-            "content": "64a8f69a1d824921eebbdf2420087937adfa45cd",
+        ("https://tdm.smugmug.com/Nature/Dove/i-kCsLJT6", {
+            "url": "f624ad7293afd6412a7d34e3950a118596c36c85",
+            "keyword": "ea70e93be5067dca988d871dcf9afac491a189a4",
+            "content": "ecbd9d7b4f75a637abc8d35319be9ec065a44eb0",
         }),
         # video
         ("https://tstravels.smugmug.com/Dailies/Daily-Dose-2015/i-39JFNzB", {
             "url": "04d0ab1ff829ca7d78f5acb5548953df08e9a5ee",
             "keyword": "c708c4b9527a2fb29396c19f7628f9cf4b0b3a39",
         }),
     )
@@ -138,20 +138,20 @@
 
 
 class SmugmugPathExtractor(SmugmugExtractor):
     """Extractor for smugmug albums from URL paths and users"""
     subcategory = "path"
     pattern = BASE_PATTERN + r"((?:/[^/?&#a-fh-mo-z][^/?&#]*)*)/?$"
     test = (
-        ("https://acapella.smugmug.com/Micro-Macro/Drops/", {
-            "pattern": "smugmug:album:ddvxpg$",
+        ("https://tdm.smugmug.com/Nature/Dove", {
+            "pattern": "smugmug:album:cr4C7f$",
         }),
-        ("https://acapella.smugmug.com/", {
+        ("https://tdm.smugmug.com/", {
             "pattern": SmugmugAlbumExtractor.pattern,
-            "url": "797eb1cbbf5ad8ecac8ee4eedc6466ed77a65d68",
+            "url": "1640028712875b90974e5aecd91b60e6de6138c7",
         }),
         # gallery node without owner
         ("https://www.smugmug.com/gallery/n-GLCjnD/", {
             "pattern": "smugmug:album:6VRT8G$",
         }),
         # custom domain
         ("smugmug:www.creativedogportraits.com/PortfolioGallery/", {
```

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/test.py` & `gallery_dl-1.9.0/gallery_dl/extractor/test.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/tsumino.py` & `gallery_dl-1.9.0/gallery_dl/extractor/tsumino.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,17 +103,17 @@
             "language"  : "English",
             "lang"      : "en",
         }
 
     def images(self, page):
         url = "{}/Read/Load/?q={}".format(self.root, self.gallery_id)
         headers = {"Referer": self.chapter_url}
-        response = self.request(url, headers=headers, expect=(404,))
+        response = self.request(url, headers=headers, fatal=False)
 
-        if response.status_code == 404:
+        if response.status_code >= 400:
             url = "{}/Read/View/{}".format(self.root, self.gallery_id)
             self.log.error(
                 "Failed to get gallery JSON data. Visit '%s' in a browser "
                 "and solve the CAPTCHA to continue.", url)
             raise exception.StopExtraction()
 
         base = self.root + "/Image/Object?name="
```

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/tumblr.py` & `gallery_dl-1.9.0/gallery_dl/extractor/tumblr.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,19 +61,23 @@
             self.api.posts_type = next(iter(self.types))
         elif not self.types:
             self.log.warning("no valid post types selected")
 
         if self.reblogs == "same-blog":
             self._skip_reblog = self._skip_reblog_same_blog
 
+        self.date_min, self.api.before = self._get_date_min_max(0, None)
+
     def items(self):
         blog = None
         yield Message.Version, 1
 
         for post in self.posts():
+            if self.date_min > post["timestamp"]:
+                return
             if post["type"] not in self.types:
                 continue
             if not blog:
                 blog = self.api.info(self.blog)
                 blog["uuid"] = self.blog
                 yield Message.Directory, blog.copy()
 
@@ -203,15 +207,15 @@
                        r"/tumblr_[^/_]+_\d+\.jpg",
             "count": 1,
             "options": (("posts", "photo"),),
         }),
         ("http://demo.tumblr.com/", {
             "pattern": (r"https?://(?:$|"
                         r"\d+\.media\.tumblr\.com/.+_1280\.jpg|"
-                        r"w+\.tumblr\.com/audio_file/demo/\d+/tumblr_\w+)"),
+                        r"a\.tumblr\.com/tumblr_\w+)"),
             "count": 3,
             "options": (("posts", "all"), ("external", True))
         }),
         ("https://mikf123-hidden.tumblr.com/", {  # dashbord-only
             "count": 2,
             "keyword": {"tags": ["test", "hidden"]},
         }),
@@ -219,14 +223,19 @@
             "count": 2,
             "keyword": {"tags": ["test", "private"]},
         }),
         ("https://mikf123-private-hidden.tumblr.com/", {  # both
             "count": 2,
             "keyword": {"tags": ["test", "private", "hidden"]},
         }),
+        ("https://mikf123.tumblr.com/", {  # date-min/-max/-format (#337)
+            "count": 4,
+            "options": (("date-min", "201804"), ("date-max", "201805"),
+                        ("date-format", "%Y%m"))
+        }),
         ("https://demo.tumblr.com/page/2"),
         ("https://demo.tumblr.com/archive"),
         ("tumblr:http://www.b-authentique.com/"),
         ("tumblr:www.b-authentique.com"),
     )
 
     def posts(self):
@@ -276,14 +285,15 @@
         ("http://demo.tumblr.com/image/459265350"),
     )
 
     def __init__(self, match):
         TumblrExtractor.__init__(self, match)
         self.post_id = match.group(3)
         self.reblogs = True
+        self.date_min = 0
 
     def posts(self):
         return self.api.posts(self.blog, {"id": self.post_id})
 
     @staticmethod
     def _setup_posttypes():
         return POST_TYPES
@@ -324,15 +334,15 @@
     """Minimal interface for the Tumblr API v2"""
     API_KEY = "O3hU2tMi5e4Qs5t3vezEi6L0qRORJ5y9oUpSGsrWu8iA3UCc3B"
     API_SECRET = "sFdsK3PDdP2QpYMRAoq0oDnw0sFS24XigXmdfnaeNZpJpqAn03"
     BLOG_CACHE = {}
 
     def __init__(self, extractor):
         oauth.OAuth1API.__init__(self, extractor)
-        self.posts_type = None
+        self.posts_type = self.before = None
 
     def info(self, blog):
         """Return general information about a blog"""
         if blog not in self.BLOG_CACHE:
             self.BLOG_CACHE[blog] = self._call(blog, "info", {})["blog"]
         return self.BLOG_CACHE[blog]
 
@@ -346,25 +356,27 @@
         return data["avatar_url"]
 
     def posts(self, blog, params):
         """Retrieve published posts"""
         params.update({"offset": 0, "limit": 50, "reblog_info": "true"})
         if self.posts_type:
             params["type"] = self.posts_type
+        if self.before:
+            params["before"] = self.before
         while True:
             data = self._call(blog, "posts", params)
             self.BLOG_CACHE[blog] = data["blog"]
             yield from data["posts"]
             params["offset"] += params["limit"]
             if params["offset"] >= data["total_posts"]:
                 return
 
     def likes(self, blog):
         """Retrieve liked posts"""
-        params = {"limit": 50}
+        params = {"limit": "50", "before": self.before}
         while True:
             posts = self._call(blog, "likes", params)["liked_posts"]
             if not posts:
                 return
             yield from posts
             params["before"] = posts[-1]["liked_timestamp"]
```

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/twitter.py` & `gallery_dl-1.9.0/gallery_dl/extractor/twitter.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # published by the Free Software Foundation.
 
 """Extract images from https://twitter.com/"""
 
 from .common import Extractor, Message
 from .. import text, exception
 from ..cache import cache
+import re
 
 
 class TwitterExtractor(Extractor):
     """Base class for twitter extractors"""
     category = "twitter"
     directory_fmt = ("{category}", "{user}")
     filename_fmt = "{tweet_id}_{num}.{extension}"
@@ -22,23 +23,29 @@
     root = "https://twitter.com"
     sizes = (":orig", ":large", ":medium", ":small")
 
     def __init__(self, match):
         Extractor.__init__(self, match)
         self.user = match.group(1)
         self.retweets = self.config("retweets", True)
+        self.content = self.config("content", False)
         self.videos = self.config("videos", False)
 
+        if self.content:
+            self._emoji_sub = re.compile(
+                r'<img class="Emoji [^>]+ alt="([^"]+)"[^>]*>').sub
+
     def items(self):
         self.login()
         yield Message.Version, 1
         yield Message.Directory, self.metadata()
 
         for tweet in self.tweets():
             data = self._data_from_tweet(tweet)
+
             if not self.retweets and data["retweet_id"]:
                 continue
 
             images = text.extract_iter(
                 tweet, 'data-image-url="', '"')
             for data["num"], url in enumerate(images, 1):
                 text.nameext_from_url(url, data)
@@ -83,26 +90,33 @@
         }
         response = self.request(url, method="POST", data=data)
 
         if "/error" in response.url:
             raise exception.AuthenticationError()
         return self.session.cookies
 
-    @staticmethod
-    def _data_from_tweet(tweet):
+    def _data_from_tweet(self, tweet):
         extr = text.extract_from(tweet)
-        return {
+        data = {
             "tweet_id"  : text.parse_int(extr('data-tweet-id="'  , '"')),
             "retweet_id": text.parse_int(extr('data-retweet-id="', '"')),
             "retweeter" : extr('data-retweeter="'  , '"'),
             "user"      : extr('data-screen-name="', '"'),
             "username"  : extr('data-name="'       , '"'),
             "user_id"   : text.parse_int(extr('data-user-id="'   , '"')),
             "date"      : text.parse_timestamp(extr('data-time="', '"')),
         }
+        if self.content:
+            content = extr('<div class="js-tweet-text-container">', '\n</div>')
+            if '<img class="Emoji ' in content:
+                content = self._emoji_sub(r"\1", content)
+            content = text.unescape(text.remove_html(content, "", ""))
+            cl, _, cr = content.rpartition("pic.twitter.com/")
+            data["content"] = cl if cl and len(cr) < 16 else content
+        return data
 
     def _tweets_from_api(self, url):
         params = {
             "include_available_features": "1",
             "include_entities": "1",
             "reset_error_state": "false",
             "lang": "en",
@@ -182,21 +196,26 @@
             "keyword": "43d98ab448193f0d4f30aa571a4b6bda9b6a5692",
         }),
         # video
         ("https://twitter.com/perrypumas/status/1065692031626829824", {
             "options": (("videos", True),),
             "pattern": r"ytdl:https://twitter.com/perrypumas/status/\d+",
         }),
+        # content with emoji, newlines, hashtags (#338)
+        ("https://twitter.com/yumi_san0112/status/1151144618936823808", {
+            "options": (("content", True),),
+            "keyword": "b13b6c4cd0b0c15b2ea7685479e7fedde3c47b9e",
+        }),
     )
 
     def __init__(self, match):
         TwitterExtractor.__init__(self, match)
         self.tweet_id = match.group(2)
 
     def metadata(self):
         return {"user": self.user, "tweet_id": self.tweet_id}
 
     def tweets(self):
         url = "{}/{}/status/{}".format(self.root, self.user, self.tweet_id)
         page = self.request(url).text
         return (text.extract(
-            page, '<div class="tweet ', '<ul class="stats')[0],)
+            page, '<div class="tweet ', 'class="js-tweet-stats-container')[0],)
```

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/vanillarock.py` & `gallery_dl-1.9.0/gallery_dl/extractor/vanillarock.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/wallhaven.py` & `gallery_dl-1.9.0/gallery_dl/extractor/wallhaven.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/warosu.py` & `gallery_dl-1.9.0/gallery_dl/extractor/warosu.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/weibo.py` & `gallery_dl-1.9.0/gallery_dl/extractor/weibo.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/wikiart.py` & `gallery_dl-1.9.0/gallery_dl/extractor/wikiart.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/xhamster.py` & `gallery_dl-1.9.0/gallery_dl/extractor/xhamster.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/xvideos.py` & `gallery_dl-1.9.0/gallery_dl/extractor/xvideos.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,47 +14,41 @@
 
 
 class XvideosExtractor(Extractor):
     """Base class for xvideos extractors"""
     category = "xvideos"
     root = "https://www.xvideos.com"
 
-    def get_page(self, url, codes=(403, 404)):
-        response = self.request(url, expect=codes)
-        if response.status_code in codes:
-            raise exception.NotFoundError(self.subcategory)
-        return response.text
-
 
 class XvideosGalleryExtractor(XvideosExtractor):
     """Extractor for user profile galleries from xvideos.com"""
     subcategory = "gallery"
     directory_fmt = ("{category}", "{user[name]}", "{title}")
     filename_fmt = "{category}_{gallery_id}_{num:>03}.{extension}"
     archive_fmt = "{gallery_id}_{num}"
     pattern = (r"(?:https?://)?(?:www\.)?xvideos\.com"
                r"/profiles/([^/?&#]+)/photos/(\d+)")
     test = (
         (("https://www.xvideos.com/profiles"
           "/pervertedcouple/photos/751031/random_stuff"), {
             "url": "4f0d992e5dc39def2c3ac8e099d17bf09e76e3c7",
-            "keyword": "8d637b372c6231cc4ada92dd5918db5fdbd06520",
+            "keyword": "65979d63a69576cf692b41d5fbbd995cc40a51b9",
         }),
         ("https://www.xvideos.com/profiles/pervertedcouple/photos/751032/", {
             "exception": exception.NotFoundError,
         }),
     )
 
     def __init__(self, match):
         XvideosExtractor.__init__(self, match)
         self.user, self.gid = match.groups()
 
     def items(self):
         url = "{}/profiles/{}/photos/{}".format(self.root, self.user, self.gid)
-        page = self.get_page(url)
+        page = self.request(url, notfound=self.subcategory).text
         data = self.get_metadata(page)
         imgs = self.get_images(page)
         data["count"] = len(imgs)
         yield Message.Version, 1
         yield Message.Directory, data
         for url in imgs:
             data["num"] = text.parse_int(url.rsplit("_", 2)[1])
@@ -109,15 +103,15 @@
 
     def __init__(self, match):
         XvideosExtractor.__init__(self, match)
         self.user = match.group(1)
 
     def items(self):
         url = "{}/profiles/{}".format(self.root, self.user)
-        page = self.get_page(url)
+        page = self.request(url, notfound=self.subcategory).text
         data = json.loads(text.extract(
             page, "xv.conf=", ";</script>")[0])["data"]
 
         if not isinstance(data["galleries"], dict):
             return
         if "0" in data["galleries"]:
             del data["galleries"]["0"]
```

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/yandere.py` & `gallery_dl-1.9.0/gallery_dl/extractor/yandere.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/yaplog.py` & `gallery_dl-1.9.0/gallery_dl/extractor/yaplog.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/extractor/yuki.py` & `gallery_dl-1.9.0/gallery_dl/extractor/yuki.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/job.py` & `gallery_dl-1.9.0/gallery_dl/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,23 +25,17 @@
             raise exception.NoExtractorError()
 
         self.extractor = extr
         extr.log.extractor = extr
         extr.log.job = self
         extr.log.debug("Using %s for '%s'", extr.__class__.__name__, extr.url)
 
-        # url predicates
-        self.pred_url = self._prepare_predicates(
-            "image", [util.UniquePredicate()], True)
-
-        # queue predicates
-        self.pred_queue = self._prepare_predicates(
-            "chapter", [], False)
+        self.pred_url = self._prepare_predicates("image", True)
+        self.pred_queue = self._prepare_predicates("chapter", False)
 
-        # category transfer
         if parent and parent.extractor.config(
                 "category-transfer", parent.extractor.categorytransfer):
             self.extractor.category = parent.extractor.category
             self.extractor.subcategory = parent.extractor.subcategory
 
         # user-supplied metadata
         self.userkwds = self.extractor.config("keywords")
@@ -138,15 +132,20 @@
     def update_kwdict(self, kwdict):
         """Update 'kwdict' with additional metadata"""
         kwdict["category"] = self.extractor.category
         kwdict["subcategory"] = self.extractor.subcategory
         if self.userkwds:
             kwdict.update(self.userkwds)
 
-    def _prepare_predicates(self, target, predicates, skip=True):
+    def _prepare_predicates(self, target, skip=True):
+        predicates = []
+
+        if self.extractor.config(target + "-unique"):
+            predicates.append(util.UniquePredicate())
+
         pfilter = self.extractor.config(target + "-filter")
         if pfilter:
             try:
                 pred = util.FilterPredicate(pfilter, target)
             except (SyntaxError, ValueError, TypeError) as exc:
                 self.extractor.log.warning(exc)
             else:
@@ -187,22 +186,26 @@
         self.sleep = None
         self.downloaders = {}
         self.postprocessors = None
         self.out = output.select()
 
     def handle_url(self, url, keywords, fallback=None):
         """Download the resource specified in 'url'"""
+        postprocessors = self.postprocessors
+        pathfmt = self.pathfmt
+        archive = self.archive
+
         # prepare download
-        self.pathfmt.set_keywords(keywords)
+        pathfmt.set_keywords(keywords)
 
-        if self.postprocessors:
-            for pp in self.postprocessors:
-                pp.prepare(self.pathfmt)
+        if postprocessors:
+            for pp in postprocessors:
+                pp.prepare(pathfmt)
 
-        if self.pathfmt.exists(self.archive):
+        if pathfmt.exists(archive):
             self.handle_skip()
             return
 
         if self.sleep:
             time.sleep(self.sleep)
 
         # download from URL
@@ -211,32 +214,32 @@
             # use fallback URLs if available
             for num, url in enumerate(fallback or (), 1):
                 self.log.info("Trying fallback URL #%d", num)
                 if self.download(url):
                     break
             else:
                 # download failed
-                self.log.error(
-                    "Failed to download %s", self.pathfmt.filename or url)
+                self.log.error("Failed to download %s",
+                               pathfmt.filename or url)
                 return
 
-        if not self.pathfmt.temppath:
+        if not pathfmt.temppath:
             self.handle_skip()
             return
 
         # run post processors
-        if self.postprocessors:
-            for pp in self.postprocessors:
-                pp.run(self.pathfmt)
+        if postprocessors:
+            for pp in postprocessors:
+                pp.run(pathfmt)
 
         # download succeeded
-        self.pathfmt.finalize()
-        self.out.success(self.pathfmt.path, 0)
-        if self.archive:
-            self.archive.add(keywords)
+        pathfmt.finalize()
+        self.out.success(pathfmt.path, 0)
+        if archive:
+            archive.add(keywords)
         self._skipcnt = 0
 
     def handle_urllist(self, urls, keywords):
         """Download the resource specified in 'url'"""
         fallback = iter(urls)
         url = next(fallback)
         self.handle_url(url, keywords, fallback)
@@ -277,36 +280,41 @@
         if downloader:
             return downloader.download(url, self.pathfmt)
         self._write_unsupported(url)
         return False
 
     def get_downloader(self, scheme):
         """Return a downloader suitable for 'scheme'"""
-        if scheme == "https":
-            scheme = "http"
         try:
             return self.downloaders[scheme]
         except KeyError:
             pass
 
         klass = downloader.find(scheme)
-        if klass and config.get(("downloader", scheme, "enabled"), True):
+        if klass and config.get(("downloader", klass.scheme, "enabled"), True):
             instance = klass(self.extractor, self.out)
         else:
             instance = None
             self.log.error("'%s:' URLs are not supported/enabled", scheme)
-        self.downloaders[scheme] = instance
+
+        if klass.scheme == "http":
+            self.downloaders["http"] = self.downloaders["https"] = instance
+        else:
+            self.downloaders[scheme] = instance
         return instance
 
     def initialize(self, keywords=None):
         """Delayed initialization of PathFormat, etc."""
         self.pathfmt = util.PathFormat(self.extractor)
         if keywords:
             self.pathfmt.set_directory(keywords)
+
         self.sleep = self.extractor.config("sleep")
+        if not self.extractor.config("download", True):
+            self.download = self.pathfmt.fix_extension
 
         skip = self.extractor.config("skip", True)
         if skip:
             self._skipexc = None
             if isinstance(skip, str):
                 skip, _, smax = skip.partition(":")
                 if skip == "abort":
```

### Comparing `gallery_dl-1.8.7/gallery_dl/oauth.py` & `gallery_dl-1.9.0/gallery_dl/oauth.py`

 * *Files 8% similar despite different names*

```diff
@@ -122,11 +122,11 @@
                 api_key, api_secret, token, token_secret)
             self.api_key = None
         else:
             self.log.debug("Using api_key authentication")
             self.session = extractor.session
             self.api_key = api_key
 
-    def request(self, url, method="GET", *, expect=range(400, 500), **kwargs):
-        kwargs["expect"] = expect
+    def request(self, url, method="GET", **kwargs):
+        kwargs["fatal"] = False
         kwargs["session"] = self.session
         return self.extractor.request(url, method, **kwargs)
```

### Comparing `gallery_dl-1.8.7/gallery_dl/option.py` & `gallery_dl-1.9.0/gallery_dl/option.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # published by the Free Software Foundation.
 
 """Command line option parsing"""
 
 import argparse
 import logging
 import json
+import sys
 from . import job, version
 
 
 class ConfigAction(argparse.Action):
     """Set argparse results as config values"""
     def __call__(self, parser, namespace, values, option_string=None):
         namespace.options.append(((self.dest,), values))
@@ -22,14 +23,22 @@
 
 class ConfigConstAction(argparse.Action):
     """Set argparse const values as config values"""
     def __call__(self, parser, namespace, values, option_string=None):
         namespace.options.append(((self.dest,), self.const))
 
 
+class DeprecatedConfigConstAction(argparse.Action):
+    """Set argparse const values as config values + deprecation warning"""
+    def __call__(self, parser, namespace, values, option_string=None):
+        print("warning: {} is deprecated. Use {} instead.".format(
+            "/".join(self.option_strings), self.choices), file=sys.stderr)
+        namespace.options.append(((self.dest,), self.const))
+
+
 class ParseAction(argparse.Action):
     """Parse <key>=<value> options and set them as config values"""
     def __call__(self, parser, namespace, values, option_string=None):
         key, _, value = values.partition("=")
         try:
             value = json.loads(value)
         except ValueError:
@@ -160,16 +169,24 @@
     downloader.add_argument(
         "-r", "--limit-rate",
         dest="rate", metavar="RATE", action=ConfigAction,
         help="Maximum download rate (e.g. 500k or 2.5M)",
     )
     downloader.add_argument(
         "-R", "--retries",
-        dest="retries", metavar="RETRIES", type=int, action=ConfigAction,
-        help="Number of retries (default: 5)",
+        dest="retries", metavar="N", type=int, action=ConfigAction,
+        help=("Maximum number of retries for failed HTTP requests "
+              "or -1 for infinite retries (default: 4)"),
+    )
+    downloader.add_argument(
+        "-A", "--abort",
+        dest="abort", metavar="N", type=int,
+        help=("Abort extractor run after N consecutive file downloads have "
+              "been skipped, e.g. if files with the same filename already "
+              "exist"),
     )
     downloader.add_argument(
         "--http-timeout",
         dest="timeout", metavar="SECONDS", type=float, action=ConfigAction,
         help="Timeout for HTTP connections (defaut: 30.0)",
     )
     downloader.add_argument(
@@ -179,23 +196,34 @@
     )
     downloader.add_argument(
         "--no-part",
         dest="part", nargs=0, action=ConfigConstAction, const=False,
         help="Do not use .part files",
     )
     downloader.add_argument(
+        "--no-mtime",
+        dest="mtime", nargs=0, action=ConfigConstAction, const=False,
+        help=("Do not set file modification times according to "
+              "Last-Modified HTTP response headers")
+    )
+    downloader.add_argument(
+        "--no-download",
+        dest="download", nargs=0, action=ConfigConstAction, const=False,
+        help=("Do not download any files")
+    )
+    downloader.add_argument(
         "--no-check-certificate",
         dest="verify", nargs=0, action=ConfigConstAction, const=False,
         help="Disable HTTPS certificate validation",
     )
     downloader.add_argument(
         "--abort-on-skip",
-        dest="skip", nargs=0, action=ConfigConstAction, const="abort",
-        help=("Abort extractor run if a file download would normally be "
-              "skipped, i.e. if a file with the same filename already exists"),
+        action=DeprecatedConfigConstAction,
+        dest="skip", nargs=0, const="abort", choices="-A/--abort",
+        help=argparse.SUPPRESS,
     )
 
     configuration = parser.add_argument_group("Configuration Options")
     configuration.add_argument(
         "-c", "--config",
         dest="cfgfiles", metavar="FILE", action="append",
         help="Additional configuration files",
@@ -290,14 +318,20 @@
     )
     postprocessor.add_argument(
         "--write-tags",
         dest="postprocessors",
         action="append_const", const={"name": "metadata", "mode": "tags"},
         help="Write image tags to separate text files",
     )
+    postprocessor.add_argument(
+        "--mtime-from-date",
+        dest="postprocessors",
+        action="append_const", const={"name": "mtime"},
+        help="Set file modification times according to 'date' metadata",
+    )
 
     parser.add_argument(
         "urls",
         metavar="URL", nargs="*",
         help=argparse.SUPPRESS,
     )
```

### Comparing `gallery_dl-1.8.7/gallery_dl/output.py` & `gallery_dl-1.9.0/gallery_dl/output.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,26 +31,50 @@
                    factory=logging._logRecordFactory):
         rv = factory(name, level, fn, lno, msg, args, exc_info, func, sinfo)
         rv.extractor = self.extractor
         rv.job = self.job
         return rv
 
 
+class Formatter(logging.Formatter):
+    """Custom formatter that supports different formats per loglevel"""
+
+    def __init__(self, fmt, datefmt):
+        if not isinstance(fmt, dict):
+            fmt = {"debug": fmt, "info": fmt, "warning": fmt, "error": fmt}
+        self.formats = fmt
+        self.datefmt = datefmt
+
+    def format(self, record):
+        record.message = record.getMessage()
+        fmt = self.formats[record.levelname]
+        if "{asctime" in fmt:
+            record.asctime = self.formatTime(record, self.datefmt)
+        msg = fmt.format_map(record.__dict__)
+        if record.exc_info and not record.exc_text:
+            record.exc_text = self.formatException(record.exc_info)
+        if record.exc_text:
+            msg = msg + "\n" + record.exc_text
+        if record.stack_info:
+            msg = msg + "\n" + record.stack_info
+        return msg
+
+
 def initialize_logging(loglevel):
     """Setup basic logging functionality before configfiles have been loaded"""
     # convert levelnames to lowercase
     for level in (10, 20, 30, 40, 50):
         name = logging.getLevelName(level)
         logging.addLevelName(level, name.lower())
 
     # register custom Logging class
     logging.Logger.manager.setLoggerClass(Logger)
 
     # setup basic logging to stderr
-    formatter = logging.Formatter(LOG_FORMAT, LOG_FORMAT_DATE, "{")
+    formatter = Formatter(LOG_FORMAT, LOG_FORMAT_DATE)
     handler = logging.StreamHandler()
     handler.setFormatter(formatter)
     handler.setLevel(loglevel)
     root = logging.getLogger()
     root.setLevel(logging.NOTSET)
     root.addHandler(handler)
 
@@ -76,38 +100,36 @@
             "%s: %s", key, exc)
         return None
     except TypeError as exc:
         logging.getLogger("gallery-dl").warning(
             "%s: missing or invalid path (%s)", key, exc)
         return None
 
-    level = opts.get("level", lvl)
-    logfmt = opts.get("format", fmt)
-    datefmt = opts.get("format-date", LOG_FORMAT_DATE)
-    formatter = logging.Formatter(logfmt, datefmt, "{")
-    handler.setFormatter(formatter)
-    handler.setLevel(level)
-
+    handler.setLevel(opts.get("level", lvl))
+    handler.setFormatter(Formatter(
+        opts.get("format", fmt),
+        opts.get("format-date", LOG_FORMAT_DATE),
+    ))
     return handler
 
 
 def configure_logging_handler(key, handler):
     """Configure a logging handler"""
     opts = config.interpolate(("output", key))
     if not opts:
         return
     if isinstance(opts, str):
         opts = {"format": opts}
     if handler.level == LOG_LEVEL and "level" in opts:
         handler.setLevel(opts["level"])
     if "format" in opts or "format-date" in opts:
-        logfmt = opts.get("format", LOG_FORMAT)
-        datefmt = opts.get("format-date", LOG_FORMAT_DATE)
-        formatter = logging.Formatter(logfmt, datefmt, "{")
-        handler.setFormatter(formatter)
+        handler.setFormatter(Formatter(
+            opts.get("format", LOG_FORMAT),
+            opts.get("format-date", LOG_FORMAT_DATE),
+        ))
 
 
 # --------------------------------------------------------------------
 # Utility functions
 
 def replace_std_streams(errors="replace"):
     """Replace standard streams and set their error handlers to 'errors'"""
```

### Comparing `gallery_dl-1.8.7/gallery_dl/postprocessor/__init__.py` & `gallery_dl-1.9.0/gallery_dl/postprocessor/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,34 +11,38 @@
 import importlib
 import logging
 
 modules = [
     "classify",
     "exec",
     "metadata",
+    "mtime",
     "ugoira",
     "zip",
 ]
 
 log = logging.getLogger("postprocessor")
 
 
 def find(name):
     """Return a postprocessor class with the given name"""
     try:
         return _cache[name]
     except KeyError:
-        klass = None
+        pass
+
+    klass = None
+    if name in modules:  # prevent unwanted imports
         try:
-            if name in modules:  # prevent unwanted imports
-                module = importlib.import_module("." + name, __package__)
-                klass = module.__postprocessor__
-        except (ImportError, AttributeError, TypeError):
+            module = importlib.import_module("." + name, __package__)
+        except ImportError:
             pass
-        _cache[name] = klass
-        return klass
+        else:
+            klass = module.__postprocessor__
+    _cache[name] = klass
+    return klass
 
 
 # --------------------------------------------------------------------
 # internals
 
 _cache = {}
```

### Comparing `gallery_dl-1.8.7/gallery_dl/postprocessor/classify.py` & `gallery_dl-1.9.0/gallery_dl/postprocessor/classify.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/postprocessor/common.py` & `gallery_dl-1.9.0/gallery_dl/postprocessor/common.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/postprocessor/exec.py` & `gallery_dl-1.9.0/gallery_dl/postprocessor/exec.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/postprocessor/metadata.py` & `gallery_dl-1.9.0/gallery_dl/postprocessor/metadata.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/postprocessor/ugoira.py` & `gallery_dl-1.9.0/gallery_dl/postprocessor/ugoira.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/postprocessor/zip.py` & `gallery_dl-1.9.0/gallery_dl/postprocessor/zip.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/gallery_dl/text.py` & `gallery_dl-1.9.0/gallery_dl/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,20 +32,23 @@
             return ""
     for char in INVALID_XML_CHARS:
         if char in xmldata:
             xmldata = xmldata.replace(char, repl)
     return xmldata
 
 
-def remove_html(txt):
+def remove_html(txt, repl=" ", sep=" "):
     """Remove html-tags from a string"""
     try:
-        return " ".join(re.sub("<[^>]+>", " ", txt).split())
+        txt = re.sub("<[^>]+>", repl, txt)
     except TypeError:
         return ""
+    if sep:
+        return sep.join(txt.split())
+    return txt.strip()
 
 
 def split_html(txt, sep=None):
     """Split input string by html-tags"""
     try:
         return [
             x.strip() for x in re.split("<[^>]+>", txt)
```

### Comparing `gallery_dl-1.8.7/gallery_dl/util.py` & `gallery_dl-1.9.0/gallery_dl/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,24 @@
 
 """Utility functions and classes"""
 
 import re
 import os
 import sys
 import json
+import time
 import shutil
 import string
 import _string
 import sqlite3
 import datetime
 import operator
 import itertools
 import urllib.parse
+from email.utils import mktime_tz, parsedate_tz
 from . import text, exception
 
 
 def bencode(num, alphabet="0123456789"):
     """Encode an integer into a base-N encoded string"""
     data = ""
     base = len(alphabet)
@@ -526,30 +528,26 @@
         self.keywords = {}
         self.filename = ""
         self.directory = self.realdirectory = ""
         self.path = self.realpath = self.temppath = ""
 
         self.basedirectory = expand_path(
             extractor.config("base-directory", (".", "gallery-dl")))
-        if os.altsep:
+        if os.altsep and os.altsep in self.basedirectory:
             self.basedirectory = self.basedirectory.replace(os.altsep, os.sep)
 
     def open(self, mode="wb"):
         """Open file and return a corresponding file object"""
         return open(self.temppath, mode)
 
     def exists(self, archive=None):
         """Return True if the file exists on disk or in 'archive'"""
-        if (archive and archive.check(self.keywords) or
-                self.has_extension and os.path.exists(self.realpath)):
-            if not self.has_extension:
-                # adjust display name
-                self.set_extension("")
-                if self.path[-1] == ".":
-                    self.path = self.path[:-1]
+        if archive and archive.check(self.keywords):
+            return self.fix_extension()
+        if self.has_extension and os.path.exists(self.realpath):
             return True
         return False
 
     def set_directory(self, keywords):
         """Build directory path and create it if necessary"""
         try:
             segments = [
@@ -584,14 +582,22 @@
 
     def set_extension(self, extension, real=True):
         """Set the 'extension' keyword"""
         self.has_extension = real
         self.keywords["extension"] = extension
         self.build_path()
 
+    def fix_extension(self, _=None):
+        if not self.has_extension:
+            self.set_extension("")
+            if self.path[-1] == ".":
+                self.path = self.path[:-1]
+                self.temppath = self.realpath = self.realpath[:-1]
+        return True
+
     def build_path(self):
         """Use filename-keywords and directory to build a full path"""
         try:
             self.filename = text.clean_path(
                 self.formatter.format_map(self.keywords))
         except Exception as exc:
             raise exception.FormatError(exc, "filename")
@@ -625,25 +631,32 @@
     def finalize(self):
         """Move tempfile to its target location"""
         if self.delete:
             self.delete = False
             os.unlink(self.temppath)
             return
 
-        if self.temppath == self.realpath:
-            return
-
-        try:
-            os.replace(self.temppath, self.realpath)
-            return
-        except OSError:
-            pass
-
-        shutil.copyfile(self.temppath, self.realpath)
-        os.unlink(self.temppath)
+        if self.temppath != self.realpath:
+            # move temp file to its actual location
+            try:
+                os.replace(self.temppath, self.realpath)
+            except OSError:
+                shutil.copyfile(self.temppath, self.realpath)
+                os.unlink(self.temppath)
+
+        if "_mtime" in self.keywords:
+            # set file modification time
+            mtime = self.keywords["_mtime"]
+            if mtime:
+                try:
+                    if isinstance(mtime, str):
+                        mtime = mktime_tz(parsedate_tz(mtime))
+                    os.utime(self.realpath, (time.time(), mtime))
+                except Exception:
+                    pass
 
     @staticmethod
     def adjust_path(path):
         """Enable longer-than-260-character paths on windows"""
         return "\\\\?\\" + os.path.abspath(path) if os.name == "nt" else path
```

### Comparing `gallery_dl-1.8.7/gallery_dl.egg-info/PKG-INFO` & `gallery_dl-1.9.0/gallery_dl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: gallery-dl
-Version: 1.8.7
+Version: 1.9.0
 Summary: Command-line program to download image-galleries and -collections from several image hosting sites
 Home-page: https://github.com/mikf/gallery-dl
 Author: Mike Fährmann
 Author-email: mike_faehrmann@web.de
 Maintainer: Mike Fährmann
 Maintainer-email: mike_faehrmann@web.de
 License: GPLv2
@@ -29,14 +29,15 @@
         - Requests_
         
         Optional
         --------
         
         - FFmpeg_: Pixiv Ugoira to WebM conversion
         - youtube-dl_: Video downloads
+        - pyOpenSSL_: Access Cloudflare protected sites
         
         
         Installation
         ============
         
         Pip
         ---
@@ -84,16 +85,16 @@
         Standalone Executable
         ---------------------
         
         Download a standalone executable file,
         put it into your `PATH <https://en.wikipedia.org/wiki/PATH_(variable)>`__,
         and run it inside a command prompt (like ``cmd.exe``).
         
-        - `Windows <https://github.com/mikf/gallery-dl/releases/download/v1.8.7/gallery-dl.exe>`__
-        - `Linux   <https://github.com/mikf/gallery-dl/releases/download/v1.8.7/gallery-dl.bin>`__
+        - `Windows <https://github.com/mikf/gallery-dl/releases/download/v1.9.0/gallery-dl.exe>`__
+        - `Linux   <https://github.com/mikf/gallery-dl/releases/download/v1.9.0/gallery-dl.bin>`__
         
         These executables include a Python 3.7 interpreter
         and all required Python packages.
         
         
         Snap
         ----
@@ -229,23 +230,24 @@
         "tokens", which should be added to your configuration file.
         
         
         .. _gallery-dl.conf:         https://github.com/mikf/gallery-dl/blob/master/docs/gallery-dl.conf
         .. _gallery-dl-example.conf: https://github.com/mikf/gallery-dl/blob/master/docs/gallery-dl-example.conf
         .. _configuration.rst:       https://github.com/mikf/gallery-dl/blob/master/docs/configuration.rst
         .. _Supported Sites:         https://github.com/mikf/gallery-dl/blob/master/docs/supportedsites.rst
-        .. _stable:                  https://github.com/mikf/gallery-dl/archive/v1.8.7.zip
+        .. _stable:                  https://github.com/mikf/gallery-dl/archive/v1.9.0.zip
         .. _dev:                     https://github.com/mikf/gallery-dl/archive/master.zip
         
         .. _Python:     https://www.python.org/downloads/
         .. _PyPI:       https://pypi.org/
         .. _pip:        https://pip.pypa.io/en/stable/
         .. _Requests:   http://docs.python-requests.org/en/master/
         .. _FFmpeg:     https://www.ffmpeg.org/
         .. _youtube-dl: https://ytdl-org.github.io/youtube-dl/
+        .. _pyOpenSSL:  https://pyopenssl.org/
         .. _Snapd:      https://docs.snapcraft.io/installing-snapd
         .. _OAuth:      https://en.wikipedia.org/wiki/OAuth
         
         .. |pypi| image:: https://img.shields.io/pypi/v/gallery-dl.svg
             :target: https://pypi.org/project/gallery-dl/
         
         .. |build| image:: https://travis-ci.org/mikf/gallery-dl.svg?branch=master
```

### Comparing `gallery_dl-1.8.7/gallery_dl.egg-info/SOURCES.txt` & `gallery_dl-1.9.0/gallery_dl.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 gallery_dl/extractor/chan.py
 gallery_dl/extractor/common.py
 gallery_dl/extractor/danbooru.py
 gallery_dl/extractor/deviantart.py
 gallery_dl/extractor/directlink.py
 gallery_dl/extractor/dynastyscans.py
 gallery_dl/extractor/e621.py
+gallery_dl/extractor/erolord.py
 gallery_dl/extractor/exhentai.py
 gallery_dl/extractor/fallenangels.py
 gallery_dl/extractor/flickr.py
 gallery_dl/extractor/foolfuuka.py
 gallery_dl/extractor/foolslide.py
 gallery_dl/extractor/gelbooru.py
 gallery_dl/extractor/gfycat.py
@@ -137,14 +138,15 @@
 gallery_dl/extractor/yaplog.py
 gallery_dl/extractor/yuki.py
 gallery_dl/postprocessor/__init__.py
 gallery_dl/postprocessor/classify.py
 gallery_dl/postprocessor/common.py
 gallery_dl/postprocessor/exec.py
 gallery_dl/postprocessor/metadata.py
+gallery_dl/postprocessor/mtime.py
 gallery_dl/postprocessor/ugoira.py
 gallery_dl/postprocessor/zip.py
 test/test_config.py
 test/test_cookies.py
 test/test_downloader.py
 test/test_extractor.py
 test/test_oauth.py
```

### Comparing `gallery_dl-1.8.7/setup.py` & `gallery_dl-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/test/test_config.py` & `gallery_dl-1.9.0/test/test_config.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/test/test_cookies.py` & `gallery_dl-1.9.0/test/test_cookies.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/test/test_downloader.py` & `gallery_dl-1.9.0/test/test_downloader.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,29 +4,99 @@
 # Copyright 2018 Mike Fährmann
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License version 2 as
 # published by the Free Software Foundation.
 
 import re
+import sys
 import base64
 import os.path
 import tempfile
-import unittest
 import threading
 import http.server
 
+import unittest
+from unittest.mock import Mock, MagicMock, patch
+
 import gallery_dl.downloader as downloader
 import gallery_dl.extractor as extractor
 import gallery_dl.config as config
 from gallery_dl.downloader.common import DownloaderBase
 from gallery_dl.output import NullOutput
 from gallery_dl.util import PathFormat
 
 
+class MockDownloaderModule(Mock):
+    __downloader__ = "mock"
+
+
+class TestDownloaderModule(unittest.TestCase):
+
+    @classmethod
+    def setUpClass(cls):
+        # allow import of ytdl downloader module without youtube_dl installed
+        sys.modules["youtube_dl"] = MagicMock()
+
+    @classmethod
+    def tearDownClass(cls):
+        del sys.modules["youtube_dl"]
+
+    def tearDown(self):
+        downloader._cache.clear()
+
+    def test_find(self):
+        cls = downloader.find("http")
+        self.assertEqual(cls.__name__, "HttpDownloader")
+        self.assertEqual(cls.scheme  , "http")
+
+        cls = downloader.find("https")
+        self.assertEqual(cls.__name__, "HttpDownloader")
+        self.assertEqual(cls.scheme  , "http")
+
+        cls = downloader.find("text")
+        self.assertEqual(cls.__name__, "TextDownloader")
+        self.assertEqual(cls.scheme  , "text")
+
+        cls = downloader.find("ytdl")
+        self.assertEqual(cls.__name__, "YoutubeDLDownloader")
+        self.assertEqual(cls.scheme  , "ytdl")
+
+        self.assertEqual(downloader.find("ftp"), None)
+        self.assertEqual(downloader.find("foo"), None)
+        self.assertEqual(downloader.find(1234) , None)
+        self.assertEqual(downloader.find(None) , None)
+
+    @patch("importlib.import_module")
+    def test_cache(self, import_module):
+        import_module.return_value = MockDownloaderModule()
+        downloader.find("http")
+        downloader.find("text")
+        downloader.find("ytdl")
+        self.assertEqual(import_module.call_count, 3)
+        downloader.find("http")
+        downloader.find("text")
+        downloader.find("ytdl")
+        self.assertEqual(import_module.call_count, 3)
+
+    @patch("importlib.import_module")
+    def test_cache_http(self, import_module):
+        import_module.return_value = MockDownloaderModule()
+        downloader.find("http")
+        downloader.find("https")
+        self.assertEqual(import_module.call_count, 1)
+
+    @patch("importlib.import_module")
+    def test_cache_https(self, import_module):
+        import_module.return_value = MockDownloaderModule()
+        downloader.find("https")
+        downloader.find("http")
+        self.assertEqual(import_module.call_count, 1)
+
+
 class TestDownloaderBase(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
         cls.extractor = extractor.find("test:")
         cls.dir = tempfile.TemporaryDirectory()
         cls.fnum = 0
@@ -130,17 +200,14 @@
 
     def test_text_download(self):
         self._run_test("text:foobar", None, "foobar", "txt", "txt")
 
     def test_text_offset(self):
         self._run_test("text:foobar", "foo", "foobar", "txt", "txt")
 
-    def test_text_extension(self):
-        self._run_test("text:foobar", None, "foobar", None, "txt")
-
     def test_text_empty(self):
         self._run_test("text:", None, "", "txt", "txt")
 
 
 class FakeDownloader(DownloaderBase):
     scheme = "fake"
```

### Comparing `gallery_dl-1.8.7/test/test_extractor.py` & `gallery_dl-1.9.0/test/test_extractor.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/test/test_oauth.py` & `gallery_dl-1.9.0/test/test_oauth.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/test/test_results.py` & `gallery_dl-1.9.0/test/test_results.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     "sankaku", "idolcomplex", "mangahere", "readcomiconline", "mangadex",
     "sankakucomplex",
 }
 
 # temporary issues, etc.
 BROKEN = {
     "komikcast",
+    "konachan",
     "mangapark",
 }
 
 
 class TestExtractorResults(unittest.TestCase):
 
     def setUp(self):
@@ -157,17 +158,18 @@
         self.list_url = []
         self.list_keyword = []
         self.list_archive = []
         self.hash_url = hashlib.sha1()
         self.hash_keyword = hashlib.sha1()
         self.hash_archive = hashlib.sha1()
         self.hash_content = hashlib.sha1()
+
         if content:
             self.fileobj = TestPathfmt(self.hash_content)
-            self.get_downloader("http")._check_extension = lambda a, b: None
+            self.get_downloader("http").check_extension = lambda a, b: None
 
         self.format_directory = TestFormatter(
             "".join(self.extractor.directory_fmt))
         self.format_filename = TestFormatter(self.extractor.filename_fmt)
 
     def run(self):
         for msg in self.extractor:
@@ -213,14 +215,15 @@
 
 class TestPathfmt():
 
     def __init__(self, hashobj):
         self.hashobj = hashobj
         self.path = ""
         self.size = 0
+        self.keywords = {}
         self.has_extension = True
 
     def __enter__(self):
         return self
 
     def __exit__(self, *args):
         pass
@@ -275,17 +278,18 @@
     config.set(("cache", "file"), ":memory:")
     config.set(("downloader", "part"), False)
     config.set(("extractor", "timeout"), 60)
     config.set(("extractor", "username"), name)
     config.set(("extractor", "password"), name)
     config.set(("extractor", "nijie", "username"), email)
     config.set(("extractor", "seiga", "username"), email)
-    config.set(("extractor", "danbooru", "username"), None)
-    config.set(("extractor", "twitter" , "username"), None)
-    config.set(("extractor", "mangoxo" , "password"), "VZ8DL3983u")
+    config.set(("extractor", "danbooru" , "username"), None)
+    config.set(("extractor", "instagram", "username"), None)
+    config.set(("extractor", "twitter"  , "username"), None)
+    config.set(("extractor", "mangoxo"  , "password"), "VZ8DL3983u")
 
     config.set(("extractor", "deviantart", "client-id"), "7777")
     config.set(("extractor", "deviantart", "client-secret"),
                "ff14994c744d9208e5caeec7aab4a026")
 
     config.set(("extractor", "tumblr", "api-key"),
                "0cXoHfIqVzMQcc3HESZSNsVlulGxEXGDTTZCDrRrjaa0jmuTc6")
```

### Comparing `gallery_dl-1.8.7/test/test_text.py` & `gallery_dl-1.9.0/test/test_text.py`

 * *Files identical despite different names*

### Comparing `gallery_dl-1.8.7/test/test_util.py` & `gallery_dl-1.9.0/test/test_util.py`

 * *Files identical despite different names*

