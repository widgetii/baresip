# Baresip Changelog

All notable changes to baresip will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).


## 2.5.0 - 2022-07-01

## What's Changed
* audio: add optional decoding buffer by @cspiel1 in https://github.com/baresip/baresip/pull/1842
* audio: RX filter thread needs separate sampv buffer by @cspiel1 in https://github.com/baresip/baresip/pull/1879
* aufile: fix possible data race warning by @cspiel1 in https://github.com/baresip/baresip/pull/1880
* audiounit,coreaudio: fix kAudioObjectPropertyElementMaster deprecation by @sreimers in https://github.com/baresip/baresip/pull/1881
* av1: explicitly check for supported OBU types by @alfredh in https://github.com/baresip/baresip/pull/1882
* audiounit/coreaudio: fix kAudioObjectPropertyElementMain by @sreimers in https://github.com/baresip/baresip/pull/1885
* ci/build: bump macos min. sdk to 10.12 by @sreimers in https://github.com/baresip/baresip/pull/1883
* ci: run only for pull requests and main branch by @sreimers in https://github.com/baresip/baresip/pull/1887
* multicast: C11 mutex by @alfredh in https://github.com/baresip/baresip/pull/1892
* dtls_srtp: enable ECC by default, remove RSA by @alfredh in https://github.com/baresip/baresip/pull/1891
* ci/build: add ubuntu 22.04 by @sreimers in https://github.com/baresip/baresip/pull/1890
* test: add check for memory leaks by @sreimers in https://github.com/baresip/baresip/pull/1896
* stream,metric: RX real-time - make metric thread-safe by @cspiel1 in https://github.com/baresip/baresip/pull/1895
* Cmake findre by @alfredh in https://github.com/baresip/baresip/pull/1893
* test: wait for both audio and video to be established by @alfredh in https://github.com/baresip/baresip/pull/1903
* docs: remove old TODO file by @alfredh in https://github.com/baresip/baresip/pull/1902
* audio: fixed check for aubuf started flag by @cspiel1 in https://github.com/baresip/baresip/pull/1904
* use new mutex interface by @cspiel1 in https://github.com/baresip/baresip/pull/1905
* audio: make rx.filtl thread-safe by @cspiel1 in https://github.com/baresip/baresip/pull/1897
* audio: allocate correct buffer size for static auplay srate by @cspiel1 in https://github.com/baresip/baresip/pull/1906
* Pulseaudio Async Interface Module by @cHuberCoffee in https://github.com/baresip/baresip/pull/1907
* Do not destroy register client when it is unregistered by @juha-h in https://github.com/baresip/baresip/pull/1908
* Two spaces are required after email address by @juha-h in https://github.com/baresip/baresip/pull/1909
* cmake: add alsa module by @alfredh in https://github.com/baresip/baresip/pull/1910
* cmake: fix static openssl and thread linking by @sreimers in https://github.com/baresip/baresip/pull/1911
* In start_registering, create register clients if reg list is empty by @juha-h in https://github.com/baresip/baresip/pull/1913
* ctrl_dbus: use new thread and mtx interface by @cspiel1 in https://github.com/baresip/baresip/pull/1916
* cmake: add pulse and pulse_async module by @cHuberCoffee in https://github.com/baresip/baresip/pull/1919
* Un-subscribe mwi at un-register by @juha-h in https://github.com/baresip/baresip/pull/1918
* call: update media on session progress. by @RobertMi21 in https://github.com/baresip/baresip/pull/1922
* ctrl_dbus send event in main thread by @cspiel1 in https://github.com/baresip/baresip/pull/1921
* uag: add timestamps to SIP trace by @cspiel1 in https://github.com/baresip/baresip/pull/1914
* main: fix open timers check by @sreimers in https://github.com/baresip/baresip/pull/1925
* cmake: add account module by @alfredh in https://github.com/baresip/baresip/pull/1926


---

## 2.4.0 - 2022-06-01

## What's Changed
* mulitcast unmute bad quality by @cspiel1 in https://github.com/baresip/baresip/pull/1821
* menu ringback for parallel call by @cspiel1 in https://github.com/baresip/baresip/pull/1827
* multicast: support error code EAGAIN of jbuf_get() by @cspiel1 in https://github.com/baresip/baresip/pull/1832
* use RTP clock rate for timestamp calculation by @cspiel1 in https://github.com/baresip/baresip/pull/1834
* av1 obu by @alfredh in https://github.com/baresip/baresip/pull/1835
* av1 packetizer by @alfredh in https://github.com/baresip/baresip/pull/1836
* av1: depacketizer by @alfredh in https://github.com/baresip/baresip/pull/1837
* Disabled debug statement by @juha-h in https://github.com/baresip/baresip/pull/1838
* h264: move from rem to re by @sreimers in https://github.com/baresip/baresip/pull/1839
* ua: send new event UA_EVENT_CREATE at successful ua allocation by @cHuberCoffee in https://github.com/baresip/baresip/pull/1840
* evdev: fix wrong ioctl size by @sreimers in https://github.com/baresip/baresip/pull/1843
* aufile: ausrc_prm has to be copied when source is allocated by @cspiel1 in https://github.com/baresip/baresip/pull/1844
* conf: missing pointer initialization found by clang analyzer by @cspiel1 in https://github.com/baresip/baresip/pull/1845
* mk/modules: fix omx RPI detection by @sreimers in https://github.com/baresip/baresip/pull/1847
* auconv: add auconv_to_float (fixes #1833) by @alfredh in https://github.com/baresip/baresip/pull/1849
* avfilter: migrate to C11 mutex by @alfredh in https://github.com/baresip/baresip/pull/1850
* avformat: C11 mutex by @alfredh in https://github.com/baresip/baresip/pull/1851
* selfview: C11 mutex by @alfredh in https://github.com/baresip/baresip/pull/1852
* audio: C11 mutex by @alfredh in https://github.com/baresip/baresip/pull/1853
* metric: C11 mutex by @alfredh in https://github.com/baresip/baresip/pull/1854
* play: C11 mutex by @alfredh in https://github.com/baresip/baresip/pull/1855
* dns: add query cache by @sreimers in https://github.com/baresip/baresip/pull/1848
* video: C11 mutex by @alfredh in https://github.com/baresip/baresip/pull/1856
* aufile: C11 threads by @alfredh in https://github.com/baresip/baresip/pull/1858
* audio: add more locking by @alfredh in https://github.com/baresip/baresip/pull/1857
* aufile/play: fix run data race by @sreimers in https://github.com/baresip/baresip/pull/1859
* mc: multicast receiver enable state fix by @cHuberCoffee in https://github.com/baresip/baresip/pull/1861
* audio: C11 thread by @alfredh in https://github.com/baresip/baresip/pull/1860
* av1: add packetize handler by @alfredh in https://github.com/baresip/baresip/pull/1865
* net/net_debug: add default route hint by @sreimers in https://github.com/baresip/baresip/pull/1864
* ice: fix local prio calculation by @sreimers in https://github.com/baresip/baresip/pull/1863
* avformat: open codec if not passthrough by @alfredh in https://github.com/baresip/baresip/pull/1866
* dtls_srtp: Minor whitespace fix by @robert-scheck in https://github.com/baresip/baresip/pull/1870
* vp8: add packetize handler by @alfredh in https://github.com/baresip/baresip/pull/1868
* vp9: add packetizer by @alfredh in https://github.com/baresip/baresip/pull/1871
* debug_cmd: support absolute path for command aufileinfo by @cspiel1 in https://github.com/baresip/baresip/pull/1875
* event: add diverter URI to UA event by @cspiel1 in https://github.com/baresip/baresip/pull/1876
* aufileinfo with synchronous response by @cspiel1 in https://github.com/baresip/baresip/pull/1877


**Full Changelog**: https://github.com/baresip/baresip/compare/v2.3.0...v2.4.0

---

## [2.3.0] - 2022-05-01

## What's Changed
* mc: multicast mute function by @cHuberCoffee in https://github.com/baresip/baresip/pull/1805
* mc: reject incoming call if high prio multicast is received by @cHuberCoffee in https://github.com/baresip/baresip/pull/1804
* mc: mcplayer stream fade-out and fade-in by @cHuberCoffee in https://github.com/baresip/baresip/pull/1802
* clean_number now will remove all non-digit chars by @mbattista in https://github.com/baresip/baresip/pull/1806
* Workflows cmakelint by @alfredh in https://github.com/baresip/baresip/pull/1808
* ccheck: check all CMakeLists.txt files by @sreimers in https://github.com/baresip/baresip/pull/1810
* mk: remove win32 MSVC project files by @alfredh in https://github.com/baresip/baresip/pull/1811
* cmake: add modules by @sreimers in https://github.com/baresip/baresip/pull/1812
* ajb,aubuf: timestamp is given in [us] by @cspiel1 in https://github.com/baresip/baresip/pull/1809
* call: allow optional leading space in SIP INFO for dtmf-relay by @thomas-karl in https://github.com/baresip/baresip/pull/1814
* conf: add fs_file_extension() by @alfredh in https://github.com/baresip/baresip/pull/1816
* Updated debian version by @juha-h in https://github.com/baresip/baresip/pull/1817
* pulse: fix timestamp integer overrun for arm by @cspiel1 in https://github.com/baresip/baresip/pull/1818
* fix audio multicast artefacts by @cspiel1 in https://github.com/baresip/baresip/pull/1819
* audio: flush aubuf if ssrc changes by @cspiel1 in https://github.com/baresip/baresip/pull/1822
* Debian control dependency update by @juha-h in https://github.com/baresip/baresip/pull/1823
* pulse: support restart of pulseaudio during stream by @cspiel1 in https://github.com/baresip/baresip/pull/1824
* version 2.3.0 by @alfredh in https://github.com/baresip/baresip/pull/1826

## New Contributors
* @thomas-karl made their first contribution in https://github.com/baresip/baresip/pull/1814

---

## [2.0.2] - 2022-04-09

## What's Changed
* Added API function call_diverteruri by @juha-h in https://github.com/baresip/baresip/pull/1780
* Avoid undeclared 'CLOCK_REALTIME' on RHEL/CentOS 7 (fixes #1781) by @robert-scheck in https://github.com/baresip/baresip/pull/1782
* audio: add lock in audio_send_digit by @GGGO in https://github.com/baresip/baresip/pull/1786
* vumeter: use new auframe_level() by @sreimers in https://github.com/baresip/baresip/pull/1788
* reg.c: use already declared acc by @GGGO in https://github.com/baresip/baresip/pull/1789
* aubuf adaptive jitter buffer by @cspiel1 in https://github.com/baresip/baresip/pull/1784
* multicast set aubuf silence by @cspiel1 in https://github.com/baresip/baresip/pull/1791
* ccheck: fix line number in error print by @cspiel1 in https://github.com/baresip/baresip/pull/1793
* test: check the correct stream in UA_EVENT_CALL_MENC by @alfredh in https://github.com/baresip/baresip/pull/1794
* audio: missing lock around stream_send by @GGGO in https://github.com/baresip/baresip/pull/1796
* docs: remove obsolete jitter_buffer_wish from config example by @cspiel1 in https://github.com/baresip/baresip/pull/1798
* Multicast jbuf and aubuf changes by @cHuberCoffee in https://github.com/baresip/baresip/pull/1797
* uag: uag_hold_resume() should not return err if there is no call to hold by @cspiel1 in https://github.com/baresip/baresip/pull/1799
* stream: remove mbuf_get_left check in rtp_handler by @GGGO in https://github.com/baresip/baresip/pull/1801
* cmake: preliminary support by @alfredh in https://github.com/baresip/baresip/pull/1800

## New Contributors
* @GGGO made their first contribution in https://github.com/baresip/baresip/pull/1786

---

## [2.0.1] - 2022-03-27

### What's Changed
* audio: fix rx_thread (adaptive jitter buffer) by @sreimers in https://github.com/baresip/baresip/pull/1769
* test: init fixture by @alfredh in https://github.com/baresip/baresip/pull/1772
* test: refactoring of test_account_uri_complete by @alfredh in https://github.com/baresip/baresip/pull/1773
* mk: check also if extensions/XShm.h is present by @cspiel1 in https://github.com/baresip/baresip/pull/1774
* menu: support custom SIP headers by @cspiel1 in https://github.com/baresip/baresip/pull/1775
* menu: use new sdp_dir_decode by @cspiel1 in https://github.com/baresip/baresip/pull/1776
* menu: avoid multiple hash entries with same key by @cspiel1 in https://github.com/baresip/baresip/pull/1777
* menu: support audio file config value "none" by @cspiel1 in https://github.com/baresip/baresip/pull/1778
* intercom: add video preview call by @cspiel1 in https://github.com/baresip/baresip/pull/1779

---

## [2.0.0] - 2022-03-11

### What's Changed
* debug_cmd: use module_event() for aufileinfo events by @cspiel1 in https://github.com/baresip/baresip/pull/1345
* multicast: use module_event() for sending events by @cspiel1 in https://github.com/baresip/baresip/pull/1346
* ctrl_dbus: use module_event() to send exported event by @cspiel1 in https://github.com/baresip/baresip/pull/1347
* ua,call: add CALL_EVENT_OUTGOING by @cspiel1 in https://github.com/baresip/baresip/pull/1348
* GTK caller history by @mbattista in https://github.com/baresip/baresip/pull/1350
* Convert FRITZ!Box XML phone book into Baresip contacts by @robert-scheck in https://github.com/baresip/baresip/pull/1382
* menu: play ringtone on audio_alert device by @cspiel1 in https://github.com/baresip/baresip/pull/1396
* menu: use str_isset() for command parameter by @cspiel1 in https://github.com/baresip/baresip/pull/1397
* dtls_srtp: use elliptic curve cryptography by @cHuberCoffee in https://github.com/baresip/baresip/pull/1385
* Support for s16 playback in jack. Needed for play tones by @srperens in https://github.com/baresip/baresip/pull/1399
* Check that account ;sipnat param has valid value by @juha-h in https://github.com/baresip/baresip/pull/1401
* Tls sipcert per acc by @cHuberCoffee in https://github.com/baresip/baresip/pull/1376
* Vidsrc add packet handler by @alfredh in https://github.com/baresip/baresip/pull/1402
* ToS for video and sip by @cspiel1 in https://github.com/baresip/baresip/pull/1393
* account: add accounts parameter to force media address family by @cspiel1 in https://github.com/baresip/baresip/pull/1395
* Selective early media by @cspiel1 in https://github.com/baresip/baresip/pull/1398
* ua,uag: split ua.c and uag.c by @cspiel1 in https://github.com/baresip/baresip/pull/1349
* Account media af template by @cspiel1 in https://github.com/baresip/baresip/pull/1406
* account: add missing client certificate parameter to template by @cHuberCoffee in https://github.com/baresip/baresip/pull/1408
* account: update answermode values in template by @cspiel1 in https://github.com/baresip/baresip/pull/1405
* menu: command uafind raises UA to head by @cspiel1 in https://github.com/baresip/baresip/pull/1407
* ctrl_dbus: fix possible memleak on failed initialization by @cspiel1 in https://github.com/baresip/baresip/pull/1410
* video passthrough by @alfredh in https://github.com/baresip/baresip/pull/1418
* menu: enable auto answer calls also for command dialdir by @cspiel1 in https://github.com/baresip/baresip/pull/1412
* menu: add command for settings media local direction by @cspiel1 in https://github.com/baresip/baresip/pull/1413
* Accounts addr params by @cspiel1 in https://github.com/baresip/baresip/pull/1414
* Accounts example cleanup by @cspiel1 in https://github.com/baresip/baresip/pull/1415
* menu,call: fix hangup for outgoing call by @cspiel1 in https://github.com/baresip/baresip/pull/1417
* multicast: add source and player API calls by @cHuberCoffee in https://github.com/baresip/baresip/pull/1403
* menu: add command /uareg by @alfredh in https://github.com/baresip/baresip/pull/1421
* menu: return complete URI for commands dial,dialdir by @cspiel1 in https://github.com/baresip/baresip/pull/1424
* menu: in command dialdir call uag_find_requri() with uri by @cspiel1 in https://github.com/baresip/baresip/pull/1425
* gst: replace variable length array (buf) with mem_zalloc by @sreimers in https://github.com/baresip/baresip/pull/1426
* menu: avoid possible memleaks for dial/dialdir commands by @cspiel1 in https://github.com/baresip/baresip/pull/1430
* uag: use local cuser for selecting user-agent (#1433) by @cspiel1 in https://github.com/baresip/baresip/pull/1434
* Work on Intercom module by @cspiel1 in https://github.com/baresip/baresip/pull/1432
* Attended Transfer on GTK by @mbattista in https://github.com/baresip/baresip/pull/1435
* Update README.md with configuration suggestion by @webstean in https://github.com/baresip/baresip/pull/1438
* README fixes by @juha-h in https://github.com/baresip/baresip/pull/1440
* Accounts examples and template by @cspiel1 in https://github.com/baresip/baresip/pull/1441
* serreg: use a timer for registration restart by @cspiel1 in https://github.com/baresip/baresip/pull/1445
* gst: audio playback not correct for some WAV files. by @RobertMi21 in https://github.com/baresip/baresip/pull/1442
* Working on intercom (ringtone override) by @cspiel1 in https://github.com/baresip/baresip/pull/1436
* Use line number 0 if user did not provide any line number by @negbie in https://github.com/baresip/baresip/pull/1451
* AMR Bandwidth Efficient mode support by @srperens in https://github.com/baresip/baresip/pull/1423
* Working on Intercom (menu: allow other modules to reject a call) by @cspiel1 in https://github.com/baresip/baresip/pull/1437
* auframe: add samplerate and channels by @sreimers in https://github.com/baresip/baresip/pull/1452
* account: comment out very basic example in template by @cspiel1 in https://github.com/baresip/baresip/pull/1458
* call answer media dir by @cspiel1 in https://github.com/baresip/baresip/pull/1449
* Account auto answer beep by @cspiel1 in https://github.com/baresip/baresip/pull/1461
* serreg: unregister correct User-Agents on registration failure by @cspiel1 in https://github.com/baresip/baresip/pull/1462
* mk: enable auto-detect of av1 module by @alfredh in https://github.com/baresip/baresip/pull/1463
* ctrl dbus makefile depends by @cspiel1 in https://github.com/baresip/baresip/pull/1457
* stream: check if media is present before enabling the RTP timeout by @cspiel1 in https://github.com/baresip/baresip/pull/1465
* ctrl_dbus: generate dbus code and documentation in makefile by @cspiel1 in https://github.com/baresip/baresip/pull/1456
* auframe: always set srate and ch by @janh in https://github.com/baresip/baresip/pull/1468
* auto answer beep per alert info URI by @cspiel1 in https://github.com/baresip/baresip/pull/1466
* auframe: move to rem by @sreimers in https://github.com/baresip/baresip/pull/1470
* mixminus: add conference feature by @sreimers in https://github.com/baresip/baresip/pull/1411
* vidbridge: check vidbridge_disp_display args fixes segfault by @sreimers in https://github.com/baresip/baresip/pull/1471
* gst: fixed some memory leaks by @RobertMi21 in https://github.com/baresip/baresip/pull/1476
* ua, menu: move auto answer delay handling to menu (#1474) by @cspiel1 in https://github.com/baresip/baresip/pull/1475
* ua,menu: move handling of ANSWERMODE_AUTO to menu (#1474) by @cspiel1 in https://github.com/baresip/baresip/pull/1478
* ausine: support for multiple samplerates by @alfredh in https://github.com/baresip/baresip/pull/1479
* account: fix IPv6 only URI for account_uri_complete() by @cspiel1 in https://github.com/baresip/baresip/pull/1472
* ilbc: remove deprecated module by @alfredh in https://github.com/baresip/baresip/pull/1483
* aubridge/device: remove unused sampv_out (old resample code) by @sreimers in https://github.com/baresip/baresip/pull/1484
* pkg-config version check by @sreimers in https://github.com/baresip/baresip/pull/1481
* mk: support more locations for libre.pc and librem.pc by @cspiel1 in https://github.com/baresip/baresip/pull/1486
* net: remove unused domain by @alfredh in https://github.com/baresip/baresip/pull/1489
* audio: fix aufilt_setup update handling by @sreimers in https://github.com/baresip/baresip/pull/1498
* SIP redirect callbackfunction by @cHuberCoffee in https://github.com/baresip/baresip/pull/1495
* add secure websocket tls context by @sreimers in https://github.com/baresip/baresip/pull/1499
* test: add stunuri by @alfredh in https://github.com/baresip/baresip/pull/1503
* turn: refactoring, add compv by @alfredh in https://github.com/baresip/baresip/pull/1505
* fmt: add string to bool function by @cspiel1 in https://github.com/baresip/baresip/pull/1501
* mk: check glib-2.0 at least like in ubuntu 18.04 by @cspiel1 in https://github.com/baresip/baresip/pull/1507
* registration fixes by @cspiel1 in https://github.com/baresip/baresip/pull/1510
* uag,menu: add commands to enable/disable UDP/TCP/TLS by @cspiel1 in https://github.com/baresip/baresip/pull/1502
* config,audio: add setting audio.telev_pt by @cspiel1 in https://github.com/baresip/baresip/pull/1509
* stream: fix telephone event (#1494) by @cspiel1 in https://github.com/baresip/baresip/pull/1506
* Fix I2S compile error, use auframe by @andreaswatch in https://github.com/baresip/baresip/pull/1512
* ci/tools: fix pylint by @sreimers in https://github.com/baresip/baresip/pull/1515
* config: not all audio config was printed by @cspiel1 in https://github.com/baresip/baresip/pull/1516
* net: replace network_if_getname with net_if_getname by @sreimers in https://github.com/baresip/baresip/pull/1518
* account: add setting audio payload type for telephone-event by @cspiel1 in https://github.com/baresip/baresip/pull/1517
* uag,menu: simplify transport enable/disable and support also ws/wss by @cspiel1 in https://github.com/baresip/baresip/pull/1514
* rst: remove deprecated module by @alfredh in https://github.com/baresip/baresip/pull/1519
* turn: add TCP and TLS transports by @alfredh in https://github.com/baresip/baresip/pull/1520
* speex_pp: remove deprecated module by @alfredh in https://github.com/baresip/baresip/pull/1521
* call: allow video calls by only rejecting a call without any common codecs by @cHuberCoffee in https://github.com/baresip/baresip/pull/1523
* multicast: add missing join for multicast addresses by @cHuberCoffee in https://github.com/baresip/baresip/pull/1524
* confg,uag: rework on sip_transports setting by @cspiel1 in https://github.com/baresip/baresip/pull/1525
* ua: check if peer is capable of video for early video by @cHuberCoffee in https://github.com/baresip/baresip/pull/1526
* mqtt/subscribe: replace fixed command buf and increase response size by @sreimers in https://github.com/baresip/baresip/pull/1527
* mqtt: add reconnect handling (lost broker connection) by @sreimers in https://github.com/baresip/baresip/pull/1528
* event: increase module_event buffer size by @sreimers in https://github.com/baresip/baresip/pull/1532
* mqtt/subscribe: use safe odict_string to prevent crashes by @sreimers in https://github.com/baresip/baresip/pull/1534
* stream: add stream_set_label by @alfredh in https://github.com/baresip/baresip/pull/1537
* Makefile dependency check improvements by @sreimers in https://github.com/baresip/baresip/pull/1531
* account: add enable/disable flag for video by @cspiel1 in https://github.com/baresip/baresip/pull/1536
* audio: use account specific audio telev pt correctly by @cspiel1 in https://github.com/baresip/baresip/pull/1542
* net: add missing HAVE_INET6 by @cspiel1 in https://github.com/baresip/baresip/pull/1543
* account: remove unused API function for video enable by @cspiel1 in https://github.com/baresip/baresip/pull/1544
* gst: changed log level for end of file message by @RobertMi21 in https://github.com/baresip/baresip/pull/1548
* multicast: add new configurable multicast TTL config parameter by @cHuberCoffee in https://github.com/baresip/baresip/pull/1545
* call: fix early video capability check (wrong SDP direction checked) by @cHuberCoffee in https://github.com/baresip/baresip/pull/1549
* audio: catch end of file message in ausrc error handler (#1539) by @RobertMi21 in https://github.com/baresip/baresip/pull/1550
* menu: added stopringing command by @RobertMi21 in https://github.com/baresip/baresip/pull/1551
* stream: remove obsolete rx.jbuf_started by @cspiel1 in https://github.com/baresip/baresip/pull/1552
* ua: downgrade level of message "ua: using best effort AF" by @viordash in https://github.com/baresip/baresip/pull/1553
* outgoing calls early callid by @cspiel1 in https://github.com/baresip/baresip/pull/1547
* audio: changed log level for ausrc error handler messages by @RobertMi21 in https://github.com/baresip/baresip/pull/1554
* SIP default protocol by @cspiel1 in https://github.com/baresip/baresip/pull/1538
* serreg: fix server selection in case all server were unavailable by @cHuberCoffee in https://github.com/baresip/baresip/pull/1557
* multicast: fix missing unlock by @alfredh in https://github.com/baresip/baresip/pull/1559
* config: replace strcpy by saver re_snprintf (#1558) by @cspiel1 in https://github.com/baresip/baresip/pull/1560
* multicast: fix coverity scan by @alfredh in https://github.com/baresip/baresip/pull/1561
* odict: hide struct odict_entry by @sreimers in https://github.com/baresip/baresip/pull/1562
* ctrl_dbus: use mqueue to trigger processing of command in remain thread by @cspiel1 in https://github.com/baresip/baresip/pull/1565
* multicast,config: add separate jitter buffer configuration by @cspiel1 in https://github.com/baresip/baresip/pull/1566
* ua: emit CALL_CLOSED event when user agent is deleted by @cspiel1 in https://github.com/baresip/baresip/pull/1564
* core: move stream_enable_rtp_timeout to api by @sreimers in https://github.com/baresip/baresip/pull/1569
* stream: add mid sdp attribute by @alfredh in https://github.com/baresip/baresip/pull/1570
* rtpext: change length type to size_t by @alfredh in https://github.com/baresip/baresip/pull/1573
* avcodec: remove old backwards compat wrapper by @alfredh in https://github.com/baresip/baresip/pull/1575
* main: Added option (-a) to set the ua agent string. by @RobertMi21 in https://github.com/baresip/baresip/pull/1576
* menu fix tones for parallel outgoing calls by @cspiel1 in https://github.com/baresip/baresip/pull/1577
* Fix win32 by @viordash in https://github.com/baresip/baresip/pull/1579
* Fix static analyzer warnings by @viordash in https://github.com/baresip/baresip/pull/1580
* call: added auto dtmf mode by @RobertMi21 in https://github.com/baresip/baresip/pull/1583
* RTP inbound telephone events should not lead to packet loss by @cspiel1 in https://github.com/baresip/baresip/pull/1581
* Running tests in a win32 project  by @viordash in https://github.com/baresip/baresip/pull/1585
* stream: wrong media direction after setting stream to hold by @RobertMi21 in https://github.com/baresip/baresip/pull/1587
* move network check to module by @cspiel1 in https://github.com/baresip/baresip/pull/1584
* serreg: do not ignore returned errors of ua_register() by @cspiel1 in https://github.com/baresip/baresip/pull/1589
* Bundle media mux by @alfredh in https://github.com/baresip/baresip/pull/1588
* mixausrc: no warnings flood when sampc changes by @cspiel1 in https://github.com/baresip/baresip/pull/1595
* ua: select laddr with route to SDP offer address by @cspiel1 in https://github.com/baresip/baresip/pull/1590
* net,uag: allow incoming peer-to-peer calls with user@domain by @cspiel1 in https://github.com/baresip/baresip/pull/1591
* uag: in uag_reset_transp() select laddr with route to SDP raddr by @cspiel1 in https://github.com/baresip/baresip/pull/1592
* uag: exit if transport could not be added by @cspiel1 in https://github.com/baresip/baresip/pull/1593
* avcodec: use const AVCodec by @alfredh in https://github.com/baresip/baresip/pull/1602
* module: deprecate module_tmp by @alfredh in https://github.com/baresip/baresip/pull/1600
* test: use ausine as audio source by @alfredh in https://github.com/baresip/baresip/pull/1601
* Selftest fakevideo by @alfredh in https://github.com/baresip/baresip/pull/1604
* When adding local address, check that it has not been added already by @juha-h in https://github.com/baresip/baresip/pull/1606
* start without network by @cspiel1 in https://github.com/baresip/baresip/pull/1607
* config: add netroam module by @sreimers in https://github.com/baresip/baresip/pull/1608
* multicast: allow any port number for sender and receiver by @cHuberCoffee in https://github.com/baresip/baresip/pull/1609
* netroam: add netlink immediate network change detection by @cspiel1 in https://github.com/baresip/baresip/pull/1612
* remove uag transp rm (#1611) by @cspiel1 in https://github.com/baresip/baresip/pull/1616
* net dns srv get by @cspiel1 in https://github.com/baresip/baresip/pull/1615
* move calls to stream_start_rtcp to call.c by @alfredh in https://github.com/baresip/baresip/pull/1617
* video: null pointer check for the display handler by @cspiel1 in https://github.com/baresip/baresip/pull/1621
* audio: add lock by @alfredh in https://github.com/baresip/baresip/pull/1619
* ua: select proper af and laddr for outgoing IP calls by @cspiel1 in https://github.com/baresip/baresip/pull/1618
* audio: lock stream by @alfredh in https://github.com/baresip/baresip/pull/1622
* test: replace mock ausrc with ausine by @alfredh in https://github.com/baresip/baresip/pull/1623
* menu ringback session progress by @cspiel1 in https://github.com/baresip/baresip/pull/1625
* New module providing webrtc aec mobile mode filter by @juha-h in https://github.com/baresip/baresip/pull/1626
* uag: respect setting sip_listen (#1627) by @cspiel1 in https://github.com/baresip/baresip/pull/1628
* select laddr for SDP with respect to net_interface by @cspiel1 in https://github.com/baresip/baresip/pull/1630
* stream: do not start audio during early-video by @cspiel1 in https://github.com/baresip/baresip/pull/1629
* remove struct media_ctx by @alfredh in https://github.com/baresip/baresip/pull/1632
* ci: add libwebrtc-audio-processing-dev (module webrtc_aec) by @sreimers in https://github.com/baresip/baresip/pull/1635
* auconv: new module for audio format conversion by @alfredh in https://github.com/baresip/baresip/pull/1634
* Support for IPv6 link local address for streams by @cspiel1 in https://github.com/baresip/baresip/pull/1624
* call: check if address family is valid also for video stream by @cspiel1 in https://github.com/baresip/baresip/pull/1636
* audio: pass pointer to tx->ausrc_prm instead of local variable by @cspiel1 in https://github.com/baresip/baresip/pull/1637
* menu: add an event for call transfer by @cspiel1 in https://github.com/baresip/baresip/pull/1641
* netroam: error handling for reset transport by @cspiel1 in https://github.com/baresip/baresip/pull/1642
* mk: use CC_TEST for auto detect modules by @sreimers in https://github.com/baresip/baresip/pull/1647
* test: use dtls_srtp.so module instead of mock by @alfredh in https://github.com/baresip/baresip/pull/1646
* stream: create jbuf only if use_rtp is set by @cspiel1 in https://github.com/baresip/baresip/pull/1648
* multicast: fix memleak in player destructor by @cspiel1 in https://github.com/baresip/baresip/pull/1653
* stream: split up sender/receiver by @alfredh in https://github.com/baresip/baresip/pull/1654
* set sdp laddr to SIP src address by @cspiel1 in https://github.com/baresip/baresip/pull/1645
* serreg fix fallback accounts by @cspiel1 in https://github.com/baresip/baresip/pull/1660
* ctrl_dbus: print command with the warning by @cspiel1 in https://github.com/baresip/baresip/pull/1662
* call: new transfer call state to handle transfered calls correctly by @cHuberCoffee in https://github.com/baresip/baresip/pull/1658
* serreg: prevent fast register retries if offline by @cspiel1 in https://github.com/baresip/baresip/pull/1663
* av1: update packetization code by @alfredh in https://github.com/baresip/baresip/pull/1657
* call: magic check in sipsess_desc_handler() by @cspiel1 in https://github.com/baresip/baresip/pull/1664
* alsa: use snd_pcm_drop instead of snd_pcm_drain by @sreimers in https://github.com/baresip/baresip/pull/1669
* Increased debian compat level to 10 by @juha-h in https://github.com/baresip/baresip/pull/1667
* conf: fix conf_configure_buf() config parse by @sreimers in https://github.com/baresip/baresip/pull/1666
* stream flush rtp socket by @cspiel1 in https://github.com/baresip/baresip/pull/1671
* Transfer like rfc5589 by @cHuberCoffee in https://github.com/baresip/baresip/pull/1678
* GTK: mem_derefer call earlier by @mbattista in https://github.com/baresip/baresip/pull/1682
* netroam: add fail counter and event by @cspiel1 in https://github.com/baresip/baresip/pull/1685
* Added API functions stream_metric_get_(tx|rx)_bitrate by @juha-h in https://github.com/baresip/baresip/pull/1686
* Multicast new functions by @cHuberCoffee in https://github.com/baresip/baresip/pull/1687
* avcodec: Enable pass-through for more codecs by @abrodkin in https://github.com/baresip/baresip/pull/1692
* menu: filter for the correct call state in menu_selcall by @cHuberCoffee in https://github.com/baresip/baresip/pull/1693
* test: fix warning on mingw32 by @alfredh in https://github.com/baresip/baresip/pull/1696
* menu: Play ringback in play device by @myrkr in https://github.com/baresip/baresip/pull/1698
* sip: add optional TCP source port by @cspiel1 in https://github.com/baresip/baresip/pull/1695
* rtpext: change id unsigned -> uint8_t by @alfredh in https://github.com/baresip/baresip/pull/1701
* ci: add mingw build test by @sreimers in https://github.com/baresip/baresip/pull/1700
* test: use mediaenc srtp instead of mock by @alfredh in https://github.com/baresip/baresip/pull/1702
* test: remove mock mediaenc by @alfredh in https://github.com/baresip/baresip/pull/1704
* descr: add session_description by @alfredh in https://github.com/baresip/baresip/pull/1706
* use fs_isfile() by @alfredh in https://github.com/baresip/baresip/pull/1709
* stream: only call rtp_clear for audio by @alfredh in https://github.com/baresip/baresip/pull/1710
* checks if call is available before calling call, closes #1708 by @mbattista in https://github.com/baresip/baresip/pull/1712
* conf: add conf_loadfile by @alfredh in https://github.com/baresip/baresip/pull/1713
* ice: remove ice_mode by @sreimers in https://github.com/baresip/baresip/pull/1714
* audio: use auframe in encode_rtp_send, ref #1699 by @alfredh in https://github.com/baresip/baresip/pull/1715
* Increased account's max video codec count from four to eight by @juha-h in https://github.com/baresip/baresip/pull/1717
* gtk: Avoid duplicate call_timer registration by @myrkr in https://github.com/baresip/baresip/pull/1719
* Attended call transfer by @cHuberCoffee in https://github.com/baresip/baresip/pull/1718
* menu: exclude given call when searching for active call by @cspiel1 in https://github.com/baresip/baresip/pull/1721
* menu: play call waiting tone on audio_player device by @cspiel1 in https://github.com/baresip/baresip/pull/1722
* ci/build/macos: link ffmpeg@4 by @sreimers in https://github.com/baresip/baresip/pull/1725
* module auresamp by @cspiel1 in https://github.com/baresip/baresip/pull/1705
* test: remove h264 testcode, already in retest by @alfredh in https://github.com/baresip/baresip/pull/1726
* h265: move from avcodec to rem by @alfredh in https://github.com/baresip/baresip/pull/1728
* mc: send more details at receiver - timeout event by @cHuberCoffee in https://github.com/baresip/baresip/pull/1731
* h265: move packetizer from avcodec to rem by @alfredh in https://github.com/baresip/baresip/pull/1732
* FFmpeg 5 by @sreimers in https://github.com/baresip/baresip/pull/1734
* Fixing clang ThreadSanitizer warnings by @sreimers in https://github.com/baresip/baresip/pull/1730
* auresamp: replace anonymous union for pre C11 compilers by @cspiel1 in https://github.com/baresip/baresip/pull/1738
* aufile: align naming of alloc handlers by @sreimers in https://github.com/baresip/baresip/pull/1739
* auresamp fixes by @cspiel1 in https://github.com/baresip/baresip/pull/1741
* mc: new priority handling with multicast state by @cHuberCoffee in https://github.com/baresip/baresip/pull/1740
* remove support for Solaris platform by @alfredh in https://github.com/baresip/baresip/pull/1745
* Allow hanging up call that has not been ACKed yet by @juha-h in https://github.com/baresip/baresip/pull/1747
* Multicast identical condition and fmt string fix by @cHuberCoffee in https://github.com/baresip/baresip/pull/1751
* audio: allocate aubuf before ausrc_alloc (fixes data race) by @sreimers in https://github.com/baresip/baresip/pull/1748
* call: send supported header for 200 answering/ok by @cHuberCoffee in https://github.com/baresip/baresip/pull/1752
* event: check if media line is present for encoding audio/video dir by @cspiel1 in https://github.com/baresip/baresip/pull/1754
* Removed unused variable in modules/webrtc_aec/aec.cpp by @juha-h in https://github.com/baresip/baresip/pull/1756
* audio use module auconv by @cspiel1 in https://github.com/baresip/baresip/pull/1742
* test: use aufile module by @alfredh in https://github.com/baresip/baresip/pull/1757
* x11grab: remove module, use avformat.so instead by @alfredh in https://github.com/baresip/baresip/pull/1758
* audio: declare iterator inside for-loop (C99) by @alfredh in https://github.com/baresip/baresip/pull/1759
* aufile: set run=true before write thread starts (#1727) by @cspiel1 in https://github.com/baresip/baresip/pull/1762
* Added new API function call_supported() and used it in menu module by @juha-h in https://github.com/baresip/baresip/pull/1761
* aufile: separate aufile_src.c from aufile.c by @cspiel1 in https://github.com/baresip/baresip/pull/1765
* ctrl_dbus: fix possible data race (#1727) by @cspiel1 in https://github.com/baresip/baresip/pull/1764
* menu select other call on hangup by @cspiel1 in https://github.com/baresip/baresip/pull/1763
* event: encode also combined media direction by @cspiel1 in https://github.com/baresip/baresip/pull/1766

## New Contributors
* @srperens made their first contribution in https://github.com/baresip/baresip/pull/1399
* @negbie made their first contribution in https://github.com/baresip/baresip/pull/1451
* @andreaswatch made their first contribution in https://github.com/baresip/baresip/pull/1512
* @viordash made their first contribution in https://github.com/baresip/baresip/pull/1553
* @abrodkin made their first contribution in https://github.com/baresip/baresip/pull/1692
* @myrkr made their first contribution in https://github.com/baresip/baresip/pull/1698

---

## [1.1.0] - 2021-04-24

- cons: emulate key-release -- ref #1329
- Correct reverse domain name notation (#1342) [#1342]
- gtk with account_uri_complete (#1339) [#1339]
- bump version to 1.1.0 -- ref #1333
- ui: fix leaking of cmd_ctx (#1338) [#1338]
- DTMF tones for A B C D (#1340) [#1340]
- account: use a fixed username for the template
- contact: update contacts template
- config: disable ctrl_dbus in config template
- Module event (#1335) [#1335]
- add event UA_EVENT_MODULE to tell to app when snapshot has been written (#1330) [#1330]
- ringtone: generated busy and ringback tone (#1332) [#1332]
- audio: prevent restart of rx_thread on call termination (#1331) [#1331]
- modules: update auplay/ausrc modules
- Auplay remove inheritance (#1328) [#1328]
- h264: add doxygen comment
- vidloop: add VIDEO_SRATE
- vidloop: check error
- vidloop: add vidframe_clear
- vidloop: split enable_codec into encoder/decoder
- Ausrc remove inheritance (#1326) [#1326]
- ua: remove prev call (#1323) [#1323]
- sndfile: get number of bytes from auframe
- plc: check format of struct auframe
- speex_pp: check format of struct auframe
- webrtc_aec: use format from struct auframe
- README: update codecs and RFCs
- menu: use uri complete for command dialdir (#1321) [#1321]
- video: check for video display before calling handler
- Changed name and made public (#1319) [#1319]
- menu: return call-id for dial and dialdir (#1320) [#1320]
- Fixes for account uri complete (#1318) [#1318]
- Avoid compiler warnings:
- Avoid compiler warnings (I haven't found anything wrong with the code)
- vidfilt: fix warning
- vidfilt: split parameters into encode/decode
- snapshot: fix warnings
- video: group functions from vidutil.c
- avfilter: fix warnings
- vumeter: use format from audio frame
- replaced ua_uri_complete with account_uri_complete (#1317) [#1317]
- aulevel: move to librem
- omx: fix warning
- vidisp: remove inheritance (#1316) [#1316]
- docs: change video settings to match the default values (#1315) [#1315]
- menu: select call in cmd_find_call() (#1314) [#1314]
- menu: use menu_stop_play() (#1311) [#1311]
- main: unload app modules in signal handler (#1310) [#1310]
- avformat: replace const double with double
- avformat: clean up ifdefs (#1313) [#1313]
- ci: drop ubuntu 16.04 support - end of life
- avformat: proper code formatting
- avcodec: add avcodec prefix to log messages
- avcodec: check length of H265 packet
- x11grab: remove vidsrc inheritance
- v4l2: remove vs inheritance
- vidsrc: remove concept of baseclass/inheritance
- ua,menu: remove uag_find_call_state (#1304) [#1304]
- Updated homepage
- sdl: correct aspect-ratio in fullscreen mode
- vidloop: add vidisp parameters
- auloop: use auframe_size
- audio: use auframe_size
- Auplay use auframe (#1305) [#1305]
- Docs examples config (#1302) [#1302]
- Serreg fixes (#1301) [#1301]
- Update config.c [#1303]
- contact: use uag_find_requri()
- ua: use new tls function to set cafile and path [#1300]
- config: add sip_capath config line
- Call event answered fixes alsa issue (#1299) [#1299]
- ctrl_dbus: send DBUS signal when dbus interface is ready (#1296) [#1296]
- Multicast call priority (#1291) [#1291]
- Menu fixes for play tones2 (#1294) [#1294]
- gst: add missing include unistd.h [#1297]
- multicast: cleanup function description and fix doxygen warning (#1292) [#1292]
- menu: remove call resume for command hangup (#1289) [#1289]
- ua: add a generic filter API for calls (#1293) [#1293]
- Merge pull request #1288 from cspiel1/remove_call_resume_on_termination [#1288]
- menu: remove call resume on termination
- multicast: fix build error when using HAVE_PTHREAD=
- alsa_play.c add suggestion to use dmix (#1283) [#1283]
- readme.md: added multicast module (#1282) [#1282]
- audiounit: fix typo
- update copyright year (#1287) [#1287]
- config cleanup (#1286) [#1286]
- update copyright year (#1285) [#1285]
- conf: add call_hold_other_calls config option (#1280) [#1280]
- config.c: added rtmp to config template (#1284) [#1284]
- main.c: update year [#1281]
- The avformat_decoder should be optional (#1277) [#1277]
- src/audio: set started false with audio_stop (#1278) [#1278]
- readme: update baresip fork links
- ausine: mono support and stereo_left/right option [#1274]
- menu: fix incoming calls are not selected on call termination (#1271) [#1271]
- test: remove mock_aucodec, using g711 instead
- opengl: remove deprecated module (#1268) [#1268]
- Added account_dtmfmode and account_set_dtmfmode API functions (#1269) [#1269]
- avcodec: remove support for MPEG4 codec
- call: start streams asynchronously (issue #1261) (#1267) [#1267]
- audio: remove special handling of Comfort Noise
- multicast: fix one doxygen warning
- menu: update doxygen comment
- menu: correct hangupall command for parallel call feature (#1264) [#1264]
- menu: on call termination select another active call (#1260) [#1260]
- ua: correct doxygen of uag_hold_resume() [#1262]
- menu: simplify cmd_hangupall() (#1259) [#1259]
- support for sending of DTMF INFO (#1258) [#1258]
- Menu optional call parameter (#1254) [#1254]
- cleanup tabs and spaces [#1256]
- ua: correct doxygen for uag_hold_others()
- ua: add doxygen for call find functions
- menu: add doxygen to cmd_hangup(), cmd_hold(), cmd_resume()
- menu: command accept searches all User-Agents for an incoming call
- ua: add function uag_find_call_state()
- menu: print correct warning for hangup, accept, hold, resume
- menu: add optional parameter call-id to cmd_call_resume()
- menu: add optional parameter call-id to cmd_call_hold()
- menu: add optional parameter call-id to cmd_hangup()
- menu: add optional parameter call-id to cmd_answerdir()
- menu: add utility function that decodes complex command parameters
- menu: use SDP_SENDRECV for cmd_answerdir() as fallback
- menu: add optional parameter call-id to cmd_answer()
- ua: add call find per call-id function
- call: call_info() prints also the call-id
- ua: in ua_print_calls() print User-Agent info in header
- menu: ua NULL check for answer command
- replace spaces with tab [#1249]
- removed newline
- undid httpreq spacing
- fixed line too long
- moved multicast template to end of config template
- ua: fix uag_hold_others use of wrong list element [#1253]
- added multicast enabled message (#1251) [#1251]
- updated date and added multicast to signaling (#1252) [#1252]
- Merge pull request #1248 from webstean/patch-2 [#1248]
- Added newline to multicast comment
- Menu ensure only one established call (#1247) [#1247]
- Call resume on hangup (#1246) [#1246]
- menu: for call answer search all UAs for calls to put on hold
- ua: ua_answer() should answer same call like ua_hold_answer()
- ua: make ua_find_call_state() global usable
- Add multicast_listener to config template (#1245) [#1245]
- Update config template to include multicast module (#1244) [#1244]
- menu: if a call becomes established then put others on hold
- ua: add uag_hold_others()
- Fix multiple resumed calls (#1242) [#1242]
- Merge pull request #1241 from cHuberCoffee/cmd_hangupall [#1241]
- RFC: Make avformat decode mjpeg v4l2 with vaapi (#1216) [#1216]
- ua: add doxygen for new uag_hold_resume()
- menu: fix missing callid of menu at call closed
- menu: use uag_hold_resume to ensure only one active call
- ua: on call resume check for other active calls
- menu: new hangupall command with direction parameter
- readme: update supported compilers and ssl libs
- menu: fix redial
- Fix spaces
- Multicast module (#1231) [#1231]
- menu: use print backend pointer pf correctly (#1222) [#1222]
- menu: start ringback only once for parallel calls (#1238) [#1238]
- jack: support port pattern in config file (#1237) [#1237]
- config: disables server verification if sip_verify_server is missing (#1236) [#1236]
- ua: for UA selection allow arbitrary aor for regint=0 accounts (#1234) [#1234]
- Ctrl dbus synchronize (#1232) [#1232]
- event: encode also remote audio direction (#1227) [#1227]
- Merge pull request #1235 from cspiel1/event_add_string_for_UA_EVENT_CUSTOM [#1235]
- event: add string for UA_EVENT_CUSTOM
- Mimic ifdef on avutil version for hwcontext
- Fix to tabs and improve checks
- src/config: show sip_cafile warning only if sip_verify_server is enabled
- Avoid compiler warnings using casts [#1228]
- test: disable SIP TLS server verification [#1224]
- config,ua: add config flag disable SIP TLS server verification
- alsa/play: snd_pcm_writei error codes are negative
- alsa: fix clang warnings "conversion loses integer precision" [#1223]
- Intelligent call answer (#1218) [#1218]
- Remove uag next (#1207) [#1207]
- Merge pull request #1219 from cspiel1/message_reply_once [#1219]
- menu: update switch_audio_player
- Make vaapi/mjpeg options of avformat
- src/config: no sip_cafile wording
- message: reply only once
- src/ua: only warn if tls_add_ca fails, same as undefined cafile [#1214]
- src/config: add sip_cafile warning and enable by default
- ua: change log message from warning to info
- video: fix video payload text
- Make avformat decode mjpeg v4l2 with vaapi
- ua: improve UA selection for incoming calls (#1206) [#1206]
- ua: limit account matches for incoming calls to non-registrar accounts
- ua: check for NULL parameter in uag_find_msg()
- ua: early exit for AF_UNSPEC in uri_match_af()
- ua: use sip_transp_decode() in uri_match_transport()
- ua: use arrays in uri_host_local()
- test: add test for deny UDP peer-to-peer call
- ua: improve UA selection for incoming calls
- Sip message to application (#1201) [#1201]
- opus: Ensure (re)init of fmtp strings (#1209) [#1209]
- ctrl_dbus: generate dbus interface during build (#1208) [#1208]
- mod_gtk: switch to gtk 3 (#1203) [#1203]
- menu: set_answer_mode: apply all uas
- menu: find_call: search all user-agents
- menu: fix usage of ua
- isac: remove deprecated module (#1204) [#1204]
- menu: cmd_print_calls: print all uas
- Fix interaction between CLI menu and GTK menu (#1202) [#1202]
- menu: rename menu_current() to menu_uacur()
- webrtc_aec: fix compilation with gcc 4.9 (fix #1193)
- win32: add cons module, fixes #1197
- ua: remove ua_aor() -- use account_aor() instead
- gtk: use account_aor()
- menu: use account_aor()
- presence: use account_aor()
- modules: use account_aor()
- account: fix video codes decode (#1196) [#1196]
- core: use account_aor()
- Merge pull request #1198 from baresip/av1 [#1198]
- Avoid unused parameter warning
- debug_cmd: add UA_EVENT_CUSTOM (#1194) [#1194]
- fix decoder changed debug text
- cairo: minor debug tuning
- menu: add uadelall to delete all user agents [#1195]
- use account_aor()
- mctrl: remove support for media-control (deprecated)
- update doxygen comments
- ua: minor cleanup
- ua: split struct uag from instance
- README: add RFC 5373
- menu: fix segfault on last account deletion (#1192) [#1192]
- call: extend SIP auto answer support for incoming calls (#1191) [#1191]
- Sip auto answer caller (#1188) [#1188]
- win32: remove timer.c
- ua: give a nice name to 'global' struct
- ua: remove ua_cur
- move uag_current to menu module
- menu: pass ua from mqtt to menu via opaque data
- Sip autoanswer callee (#1187) [#1187]
- ua: for answer-mode early also send INCOMING event (#1185) [#1185]
- gst: The error handler call for end of stream is now (#1182) [#1182]
- mk: also detect mqtt.so in SYSROOT_ALT
- contact: add ua_lookup_domain
- video: minor tuning of pipeline text
- gst: playback of read only audio files failed (#1183) [#1183]
- gtk: make a local pointer to current ua
- menu: clean up usage of uag_current()
- call: correction of remote video direction info at SDP-offer (#1181) [#1181]
- debug_cmd: print all user-agents
- presence: one command with status as argument
- ua: rename presence status to pstat
- ua: remove LIBRE_HAVE_SIPTRACE check, always enabled
- update doxygen comments
- mk: update doxygen config file
- menu: initialize menu with zeros (#1179) [#1179]
- Re mk cross build2 (#1161) [#1161]
- net: make fallback DNS ignored message debug only
- mixausrc: improve logging [#1176]
- mixausrc: fix shorten-64-to-32 warnings
- config: template for osx/ios
- Supressed clang zero length array warning
- Added ctx param to video_stop/video_stop_source and set ctx to null (#1173) [#1173]
- avformat: add empty line after base class
- Make macos warnings into errors (#1171) [#1171]
- disable mixausrc until warnings are fixed
- clang shorten-64-to-32 warnings (#1170) [#1170]
- Mixausrc (#1159) [#1159]
- aufile: fix warning on OSX
- alsa: print warning if running, fixed #1162
- Don't default stunuser/pass to account authuser/pass (#1164) [#1164]
- Audio file info (#1157) [#1157]
- gitignore: clangd cache, compile_commands.json and cleanup
- Merge pull request #1167 from baresip/video_display [#1167]
- Reordered video_stop_display
- Expose video_stop_display() to API
- Video dir rename (#1158) [#1158]
- ci: use baresip/rem repo
- stream: add function to send a RTP dummy packet (#1156) [#1156]
- Play aufile extended support (#1155) [#1155]
- video: move video related start/stop/update into video file (#1151) [#1151]
- aufile: add audio player to write speaker data to wav file (#1153) [#1153]
- Fix compiler warnings (#1152) [#1152]
- play: fix warning
- play ausrc (#1147) [#1147]
- README: add more status badges
- README: replace travis status badge
- menu: fix uint16_t scode [#1149]
- config: revert dirent.h changes
- audio: fix HAVE_PTHREAD audio_destructor
- gst ready for file play (#1148) [#1148]
- debug_cmd: mem_deref of player fixes segfault (#1146) [#1146]
- net: remove deprecated net_domain()
- update contact examples
- fix freeze on hangup (#1135) (#1145) [#1145]
- menu: make audio files configurable (#1144) [#1144]
- aptx: declare variable outside for-loop
- fix warnings on openbsd
- jack: declare variable outside for loop
- account: declare variable outside for loop
- coreaudio: declare variable outside for loop
- menu: initialize menu.play fixes segfault (#1143) [#1143]
- ausine: declare variable outside for loop
- timer: remove tmr_jiffies_usec (replaced by libre) (#1141) [#1141]
- Adaptive jbuf (#1112) [#1112]
- Update build.yml (#1140) [#1140]
- mqtt: allow to separate pub from sub topic base (#1139) [#1139]
- video: fix warning
- mqtt: fix printing port and add tls support (#1138) [#1138]
- httpreq: in cmd_setauth check if parameter was given (#1134) [#1134]
- Merge pull request #1132 from baresip/pr-dependency-action [#1132]
- ci: add pull request dependency checkouts
- audio: remove redundant union
- menu: use menu_ as prefix for global symbols
- menu: use menu_ as prefix for global symbols
- ci: add apt-get update
- menu: module refactoring (#1129) [#1129]
- audio, video, stream: check payload type before put to jbuf (#1128) [#1128]
- Cmd dialdir (#1126) [#1126]
- Cmd acceptdir (#1125) [#1125]
- event: add register fallback to event string and class name (#1124) [#1124]
- avformat: use %u for unsigned
- modify event type and check if peeruri null  (#1119) [#1119]
- event: move code from ua.c (#1118) [#1118]
- Valgrind ci (#1117) [#1117]
- h264 cleanup, second part (#1115) [#1115]
- h264 cleanup (#1114) [#1114]
- Merge pull request #1113 from baresip/github-actions-v2 [#1113]
- ci: remove travis
- ci: add github actions - replaces travisci
- qtcapture: remove deprecated module (#1107) [#1107]
- test: prepare for dualstack
- test: add mock dns_server_add_aaaa
- make EXTRA_MODULES last, not first (#1106) [#1106]
- httpreq: fix cmd_settimeout
- test: bind network to localhost, a fix for #1090
- modules/webrtc_aec: link flags fixes (#1105) [#1105]
- menu: commands in alphabetical order
- httpreq: fix warning about unused args
- serreg: fix warnings about unused argument
- menu: fix warnings about unused argument
- Add a HTTP request module with authorization (#1099) [#1099]
- Menu: corrections for ring tones and call status by means of a global call counter (#1102) [#1102]
- mk: remove dirent.h
- Updating .vcxproj file for windows builds (#1097) [#1097]
- ccheck: change license to BSD license
- Merge pull request #1095 from baresip/websocket [#1095]
- Serial registration (#1083) [#1083]
- Ctrl dbus (#1085) [#1085]
- README: remove references to creytiv.com
- Branch of baresip that includes Alfred's sip websocket patch
- Merge pull request #1091 from baresip/debian [#1091]
- ua, menu: new command to print certificate issuer and subject (#1078) [#1078]
- .gitignore: add ctags and Vim swp files (#1084) [#1084]


### Contributors (many thanks)

- [alfredh](https://github.com/alfredh)
- [robert-scheck](https://github.com/robert-scheck)
- [mbattista](https://github.com/mbattista)
- [cspiel1](https://github.com/cspiel1)
- [juha-h](https://github.com/juha-h)
- [ahinrichs](https://github.com/ahinrichs)
- [jurjen-van-dijk](https://github.com/jurjen-van-dijk)
- [sreimers](https://github.com/sreimers)
- [cHuberCoffee](https://github.com/cHuberCoffee)
- [webstean](https://github.com/webstean)
- [viric](https://github.com/viric)
- [agramner](https://github.com/agramner)
- [weili-jiang](https://github.com/weili-jiang)
- [thillux](https://github.com/thillux)
- [wkiswk](https://github.com/wkiswk)
- [philippbachmann08](https://github.com/philippbachmann08)
- [ursfassler](https://github.com/ursfassler)
- [RobertMi21](https://github.com/RobertMi21)
- [alberanid](https://github.com/alberanid)
- [agranig](https://github.com/agranig)
- [nanguantong](https://github.com/nanguantong)
- [johnjuuljensen](https://github.com/johnjuuljensen)

---

## [1.0.0] - 2020-09-11

### Added

- aac: add AAC_STREAMTYPE_AUDIO enum value
- aac: add AAC_ prefix
- Video mode param to call_answer(), ua_answer() and ua_hold_answer [#966]
- video_stop_display() API function [#977]
- module: add path to module_load() function
- conf: add conf_configure_buf
- test: add usage of g711.so module [#978]
- JSON initial codec state command and response [#973]
- account_set_video_codecs() API function [#981]
- net: add fallback dns nameserver [#996]
- gtk: show call_peername in notify title [#1006]
- call: Added call_state() API function that returns enum state of the call [#1013]
- account_set_stun_user() and account_set_stun_pass() API functions [#1015]
- API functions account_stun_uri and account_set_stun_uri. [#1018]
- ausine: Audio sine wave input module [#1021]
- gtk/menu: replace spaces from uri [#1007]
- jack: allowing jack client name to be specified in the config file [#1025] [#1020]
- snapshot: Add snapshot_send and snapshot_recv commands [#1029]
- webrtc_aec: 'extended_filter' config option [#1030]
- avfilter: FFmpeg filter graphs integration [#1038]
- reg: view proxy expiry value in reg_status [#1068]
- account: add parameter rwait for re-register interval [#1069]
- call, stream, menu: add cmd to set the direction of video stream [#1073]
- Added AMRWBENC_PATH env var to amr module module.mk [#1081]

### Changed

- **Using [baresip/re](https://github.com/baresip/re) fork now**
- audio: move calculation to audio_jb_current_value
- avformat: clean up docs
- gzrtp: update docs
- account: increased size of audio codec list to 16
- video: make video_sdp_attr_decode public
- config: Derive default audio driver from default audio device [#1009]
- jack: modifying info message on jack client creation [#1019]
- call: when video stream is disabled, stop also video display [#1023]
- dtls_srtp: use tls_set_selfsigned_rsa with keysize 2048 [#1062] [#1056]
- rst: use a min ptime of 20ms
- aac: change ptime to 4ms

### Fixed

- avcodec: fix H.264 interop with Firefox
- winwave: waveInGetPosition is no longer supported for use as of Windows Vista [#960]
- avcodec: call av_hwdevice_ctx_create before if-statement
- account: use single quote instead of backtick
- ice: fix segfault in connh [#980]
- call: Update call->got_offer when re-INVITE or answer to re-INVITE
  is received [#986]
- mk: Test also for /usr/lib64/libspeexdsp.so to cover Fedora/RHEL/CentOS [#992]
- config: Allow distribution specific CA trust bundle locations (fixes [#993]
- config: Allow distribution specific default audio device (fixes [#994]
- mqtt: fix err is never read (found by clang static analyzer)
- avcodec: fix err is never read (found by clang static analyzer)
- gtk: notification buttons do not work on Systems [#1012]
- gtk: fix dtmf_tone and add tones as feedback [#1010]
- pulse: drain pulse buffers before freeing [#1016]
- jack: jack_play connect all physical ports [#1028]
- Makefile: do not try to install modules if build is static [#1031]
- gzrtp: media_alloc function is missing [#1034] [#1022]
- call: when updating video, check if video stream has been disabled [#1037]
- amr: fix length check, fixes [#1011]
- modules: fix search path for avdevice.h [#1043]
- gtk: declare variables C89 style
- config: init newly added member
- menu: fix segfault in ua_event_handler [#1059] [#1061]
- debug_cmd: fix OpenSSL no-deprecated [#1065]
- aac: handle missing bitrate parameter in SDP format
- av1: properly configure encoder
- call: When terminating outgoing call, terminate also possible refer
  subscription [#1082]
- menu: fix segfault in /aubitrate command
- amr: should check if file (instead of directory) exists

### Removed

- ice: remove support for ICE-lite
- ice: remove ice_debug, use log level DEBUG instead
- ice: make stun server optional
- config: remove ice_debug option (unused)
- opengles: remove module (not working) [#1079]

### Contributors (many thanks)

- Alfred E. Heggestad
- Alexander Gramner
- Andrew Webster
- Christian Spielberger
- Christoph Huber
- Davide Alberani
- Ethan Funk
- Juha Heinanen
- mbattista
- Michael Malone
- Mikl Kurkov
- ndilieto
- Robert Scheck
- Roger Sandholm
- Sebastian Reimers


[#960]: https://github.com/baresip/baresip/pull/960
[#966]: https://github.com/baresip/baresip/pull/966
[#973]: https://github.com/baresip/baresip/pull/973
[#977]: https://github.com/baresip/baresip/pull/977
[#978]: https://github.com/baresip/baresip/pull/978
[#980]: https://github.com/baresip/baresip/pull/980
[#981]: https://github.com/baresip/baresip/pull/981
[#986]: https://github.com/baresip/baresip/pull/986
[#992]: https://github.com/baresip/baresip/pull/992
[#993]: https://github.com/baresip/baresip/pull/993
[#994]: https://github.com/baresip/baresip/pull/994
[#996]: https://github.com/baresip/baresip/pull/996
[#1006]: https://github.com/baresip/baresip/pull/1006
[#1007]: https://github.com/baresip/baresip/pull/1007
[#1009]: https://github.com/baresip/baresip/pull/1009
[#1010]: https://github.com/baresip/baresip/pull/1010
[#1011]: https://github.com/baresip/baresip/pull/1011
[#1012]: https://github.com/baresip/baresip/pull/1012
[#1013]: https://github.com/baresip/baresip/pull/1013
[#1015]: https://github.com/baresip/baresip/pull/1015
[#1016]: https://github.com/baresip/baresip/pull/1016
[#1018]: https://github.com/baresip/baresip/pull/1018
[#1019]: https://github.com/baresip/baresip/pull/1019
[#1020]: https://github.com/baresip/baresip/pull/1020
[#1021]: https://github.com/baresip/baresip/pull/1021
[#1022]: https://github.com/baresip/baresip/pull/1022
[#1023]: https://github.com/baresip/baresip/pull/1023
[#1025]: https://github.com/baresip/baresip/pull/1025
[#1028]: https://github.com/baresip/baresip/pull/1028
[#1029]: https://github.com/baresip/baresip/pull/1029
[#1030]: https://github.com/baresip/baresip/pull/1030
[#1031]: https://github.com/baresip/baresip/pull/1031
[#1034]: https://github.com/baresip/baresip/pull/1034
[#1037]: https://github.com/baresip/baresip/pull/1037
[#1038]: https://github.com/baresip/baresip/pull/1038
[#1043]: https://github.com/baresip/baresip/pull/1043
[#1056]: https://github.com/baresip/baresip/pull/1056
[#1059]: https://github.com/baresip/baresip/pull/1059
[#1061]: https://github.com/baresip/baresip/pull/1061
[#1062]: https://github.com/baresip/baresip/pull/1062
[#1065]: https://github.com/baresip/baresip/pull/1065
[#1068]: https://github.com/baresip/baresip/pull/1068
[#1069]: https://github.com/baresip/baresip/pull/1069
[#1073]: https://github.com/baresip/baresip/pull/1073
[#1078]: https://github.com/baresip/baresip/pull/1078
[#1079]: https://github.com/baresip/baresip/pull/1079
[#1081]: https://github.com/baresip/baresip/pull/1081
[#1082]: https://github.com/baresip/baresip/pull/1082
[#1083]: https://github.com/baresip/baresip/pull/1083
[#1084]: https://github.com/baresip/baresip/pull/1084
[#1085]: https://github.com/baresip/baresip/pull/1085
[#1091]: https://github.com/baresip/baresip/pull/1091
[#1095]: https://github.com/baresip/baresip/pull/1095
[#1097]: https://github.com/baresip/baresip/pull/1097
[#1099]: https://github.com/baresip/baresip/pull/1099
[#1102]: https://github.com/baresip/baresip/pull/1102
[#1105]: https://github.com/baresip/baresip/pull/1105
[#1106]: https://github.com/baresip/baresip/pull/1106
[#1107]: https://github.com/baresip/baresip/pull/1107
[#1112]: https://github.com/baresip/baresip/pull/1112
[#1113]: https://github.com/baresip/baresip/pull/1113
[#1114]: https://github.com/baresip/baresip/pull/1114
[#1115]: https://github.com/baresip/baresip/pull/1115
[#1117]: https://github.com/baresip/baresip/pull/1117
[#1118]: https://github.com/baresip/baresip/pull/1118
[#1119]: https://github.com/baresip/baresip/pull/1119
[#1124]: https://github.com/baresip/baresip/pull/1124
[#1125]: https://github.com/baresip/baresip/pull/1125
[#1126]: https://github.com/baresip/baresip/pull/1126
[#1128]: https://github.com/baresip/baresip/pull/1128
[#1129]: https://github.com/baresip/baresip/pull/1129
[#1132]: https://github.com/baresip/baresip/pull/1132
[#1134]: https://github.com/baresip/baresip/pull/1134
[#1138]: https://github.com/baresip/baresip/pull/1138
[#1139]: https://github.com/baresip/baresip/pull/1139
[#1140]: https://github.com/baresip/baresip/pull/1140
[#1141]: https://github.com/baresip/baresip/pull/1141
[#1143]: https://github.com/baresip/baresip/pull/1143
[#1144]: https://github.com/baresip/baresip/pull/1144
[#1145]: https://github.com/baresip/baresip/pull/1145
[#1146]: https://github.com/baresip/baresip/pull/1146
[#1147]: https://github.com/baresip/baresip/pull/1147
[#1148]: https://github.com/baresip/baresip/pull/1148
[#1149]: https://github.com/baresip/baresip/pull/1149
[#1151]: https://github.com/baresip/baresip/pull/1151
[#1152]: https://github.com/baresip/baresip/pull/1152
[#1153]: https://github.com/baresip/baresip/pull/1153
[#1155]: https://github.com/baresip/baresip/pull/1155
[#1156]: https://github.com/baresip/baresip/pull/1156
[#1157]: https://github.com/baresip/baresip/pull/1157
[#1158]: https://github.com/baresip/baresip/pull/1158
[#1159]: https://github.com/baresip/baresip/pull/1159
[#1161]: https://github.com/baresip/baresip/pull/1161
[#1164]: https://github.com/baresip/baresip/pull/1164
[#1167]: https://github.com/baresip/baresip/pull/1167
[#1170]: https://github.com/baresip/baresip/pull/1170
[#1171]: https://github.com/baresip/baresip/pull/1171
[#1173]: https://github.com/baresip/baresip/pull/1173
[#1176]: https://github.com/baresip/baresip/pull/1176
[#1179]: https://github.com/baresip/baresip/pull/1179
[#1181]: https://github.com/baresip/baresip/pull/1181
[#1182]: https://github.com/baresip/baresip/pull/1182
[#1183]: https://github.com/baresip/baresip/pull/1183
[#1185]: https://github.com/baresip/baresip/pull/1185
[#1187]: https://github.com/baresip/baresip/pull/1187
[#1188]: https://github.com/baresip/baresip/pull/1188
[#1191]: https://github.com/baresip/baresip/pull/1191
[#1192]: https://github.com/baresip/baresip/pull/1192
[#1194]: https://github.com/baresip/baresip/pull/1194
[#1195]: https://github.com/baresip/baresip/pull/1195
[#1196]: https://github.com/baresip/baresip/pull/1196
[#1198]: https://github.com/baresip/baresip/pull/1198
[#1201]: https://github.com/baresip/baresip/pull/1201
[#1202]: https://github.com/baresip/baresip/pull/1202
[#1203]: https://github.com/baresip/baresip/pull/1203
[#1204]: https://github.com/baresip/baresip/pull/1204
[#1206]: https://github.com/baresip/baresip/pull/1206
[#1207]: https://github.com/baresip/baresip/pull/1207
[#1208]: https://github.com/baresip/baresip/pull/1208
[#1209]: https://github.com/baresip/baresip/pull/1209
[#1214]: https://github.com/baresip/baresip/pull/1214
[#1216]: https://github.com/baresip/baresip/pull/1216
[#1218]: https://github.com/baresip/baresip/pull/1218
[#1219]: https://github.com/baresip/baresip/pull/1219
[#1222]: https://github.com/baresip/baresip/pull/1222
[#1223]: https://github.com/baresip/baresip/pull/1223
[#1224]: https://github.com/baresip/baresip/pull/1224
[#1227]: https://github.com/baresip/baresip/pull/1227
[#1228]: https://github.com/baresip/baresip/pull/1228
[#1231]: https://github.com/baresip/baresip/pull/1231
[#1232]: https://github.com/baresip/baresip/pull/1232
[#1234]: https://github.com/baresip/baresip/pull/1234
[#1235]: https://github.com/baresip/baresip/pull/1235
[#1236]: https://github.com/baresip/baresip/pull/1236
[#1237]: https://github.com/baresip/baresip/pull/1237
[#1238]: https://github.com/baresip/baresip/pull/1238
[#1241]: https://github.com/baresip/baresip/pull/1241
[#1242]: https://github.com/baresip/baresip/pull/1242
[#1244]: https://github.com/baresip/baresip/pull/1244
[#1245]: https://github.com/baresip/baresip/pull/1245
[#1246]: https://github.com/baresip/baresip/pull/1246
[#1247]: https://github.com/baresip/baresip/pull/1247
[#1248]: https://github.com/baresip/baresip/pull/1248
[#1249]: https://github.com/baresip/baresip/pull/1249
[#1251]: https://github.com/baresip/baresip/pull/1251
[#1252]: https://github.com/baresip/baresip/pull/1252
[#1253]: https://github.com/baresip/baresip/pull/1253
[#1254]: https://github.com/baresip/baresip/pull/1254
[#1256]: https://github.com/baresip/baresip/pull/1256
[#1258]: https://github.com/baresip/baresip/pull/1258
[#1259]: https://github.com/baresip/baresip/pull/1259
[#1260]: https://github.com/baresip/baresip/pull/1260
[#1262]: https://github.com/baresip/baresip/pull/1262
[#1264]: https://github.com/baresip/baresip/pull/1264
[#1267]: https://github.com/baresip/baresip/pull/1267
[#1268]: https://github.com/baresip/baresip/pull/1268
[#1269]: https://github.com/baresip/baresip/pull/1269
[#1271]: https://github.com/baresip/baresip/pull/1271
[#1274]: https://github.com/baresip/baresip/pull/1274
[#1277]: https://github.com/baresip/baresip/pull/1277
[#1278]: https://github.com/baresip/baresip/pull/1278
[#1280]: https://github.com/baresip/baresip/pull/1280
[#1281]: https://github.com/baresip/baresip/pull/1281
[#1282]: https://github.com/baresip/baresip/pull/1282
[#1283]: https://github.com/baresip/baresip/pull/1283
[#1284]: https://github.com/baresip/baresip/pull/1284
[#1285]: https://github.com/baresip/baresip/pull/1285
[#1286]: https://github.com/baresip/baresip/pull/1286
[#1287]: https://github.com/baresip/baresip/pull/1287
[#1288]: https://github.com/baresip/baresip/pull/1288
[#1289]: https://github.com/baresip/baresip/pull/1289
[#1291]: https://github.com/baresip/baresip/pull/1291
[#1292]: https://github.com/baresip/baresip/pull/1292
[#1293]: https://github.com/baresip/baresip/pull/1293
[#1294]: https://github.com/baresip/baresip/pull/1294
[#1296]: https://github.com/baresip/baresip/pull/1296
[#1297]: https://github.com/baresip/baresip/pull/1297
[#1299]: https://github.com/baresip/baresip/pull/1299
[#1300]: https://github.com/baresip/baresip/pull/1300
[#1301]: https://github.com/baresip/baresip/pull/1301
[#1302]: https://github.com/baresip/baresip/pull/1302
[#1303]: https://github.com/baresip/baresip/pull/1303
[#1304]: https://github.com/baresip/baresip/pull/1304
[#1305]: https://github.com/baresip/baresip/pull/1305
[#1310]: https://github.com/baresip/baresip/pull/1310
[#1311]: https://github.com/baresip/baresip/pull/1311
[#1313]: https://github.com/baresip/baresip/pull/1313
[#1314]: https://github.com/baresip/baresip/pull/1314
[#1315]: https://github.com/baresip/baresip/pull/1315
[#1316]: https://github.com/baresip/baresip/pull/1316
[#1317]: https://github.com/baresip/baresip/pull/1317
[#1318]: https://github.com/baresip/baresip/pull/1318
[#1319]: https://github.com/baresip/baresip/pull/1319
[#1320]: https://github.com/baresip/baresip/pull/1320
[#1321]: https://github.com/baresip/baresip/pull/1321
[#1323]: https://github.com/baresip/baresip/pull/1323
[#1326]: https://github.com/baresip/baresip/pull/1326
[#1328]: https://github.com/baresip/baresip/pull/1328
[#1330]: https://github.com/baresip/baresip/pull/1330
[#1331]: https://github.com/baresip/baresip/pull/1331
[#1332]: https://github.com/baresip/baresip/pull/1332
[#1335]: https://github.com/baresip/baresip/pull/1335
[#1338]: https://github.com/baresip/baresip/pull/1338
[#1339]: https://github.com/baresip/baresip/pull/1339
[#1340]: https://github.com/baresip/baresip/pull/1340
[#1342]: https://github.com/baresip/baresip/pull/1342


[Unreleased]: https://github.com/baresip/baresip/compare/v2.3.0...HEAD
[2.3.0]: https://github.com/baresip/baresip/compare/v2.0.2...v2.3.0
[2.0.2]: https://github.com/baresip/baresip/compare/v2.0.1...v2.0.2
[2.0.1]: https://github.com/baresip/baresip/compare/v2.0.0...v2.0.1
[2.0.0]: https://github.com/baresip/baresip/compare/v1.1.0...v2.0.0
[1.1.0]: https://github.com/baresip/baresip/compare/v1.0.0...v1.1.0
[1.0.0]: https://github.com/baresip/baresip/compare/v0.6.6...v1.0.0
