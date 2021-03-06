History
=======

## 0.13.1

* Do not duplicate messages over a single client
  [#44](https://github.com/mcollina/mosca/issues/63).

## 0.13.0

* mqtt over websocket support.
  [#44](https://github.com/mcollina/mosca/issues/44).
* MongoDB persistence deletes old retained messages
  [#61](https://github.com/mcollina/mosca/issues/61).

## 0.12.1

* Support both a config file and command-line options,
  fixes [#58](https://github.com/mcollina/mosca/issues/58) and
  [#60](https://github.com/mcollina/mosca/issues/60).
* Fixes redis persistence for unknown client ids
  [#59](https://github.com/mcollina/mosca/pull#59).

## 0.12.0

* Close forcefully a connecting client
  [#57](https://github.com/mcollina/mosca/pull/57) by
  (@chriswiggins)[https://github.com/chriswiggins].
* Updated LevelUp to 0.16.0.
* Updated Level-Sublevel to 5.1.1.
* Better persistence for the subscriptions.

## 0.11.0

* TLS support thanks to (@samirnaik)[https://github.com/samirnaik].
* Send dup flag for resent messages.

## 0.10.0

* Updated MQTT.js to v0.3.0.

## 0.9.5

* Consistent support of the "ready" callback in the persistences
  implementations (Memory and Mongo).
* Fixed loading of a config file from an absolute path.
* README fixes.

## 0.9.4

* New README, thanks to [Andrea Reginato](https://github.com/andreareginato).
* Removed explicit dependency to level-fix-range, as the original bug
  was solved in level-sublevel v4.8.1.

## 0.9.3

* Upgraded LevelUp to 0.12.0.
* Fixed level-fix-range dependency to avoid a bug
  https://github.com/dominictarr/level-sublevel/issues/21.
* Improved Logger creation in Server.
* Improved Logger handling inside clients.

## 0.9.2

* Added the ability to pass a custom Ascoltatore to `mosca.Server`.
* `mosca.Server` callbacks now yields the server.
* `mosca.Server` can now be called like a function.

## 0.9.1

* 'test/topic' is different from '/test/topic'
* Resetting ping timer on publish, subcribe, unsubscribe:
  [#47](https://github.com/mcollina/mosca/pull/47).

## 0.9.0

* Bumped Ascoltatori to 0.11.0.
* Improved logging for each client.
* Fixed multiple topic naming, mainly 'test/topic' and 'test/topic/'
  should be the same
  [#46](https://github.com/mcollina/mosca/pull/46).
* Better handling of defaults 
  [#39](https://github.com/mcollina/mosca/pull/39).
* Enforcing client identifier length
  [#33](https://github.com/mcollina/mosca/pull/33).

## 0.8.2

* Passing the correct Client object to `authorizePublish`,
  [#43](https://github.com/mcollina/mosca/pull/43).

## 0.8.1

* Refactored the Server-Persistence wiring interface
  to solve some spurious test failures.

## 0.8.0

* Updated Ascoltatori to 0.8.0.

## 0.7.3

* Fixed MongoDB persistance tests on Travis.
* Fixed spurious errors in Redis persistance.

## 0.7.2

* More README fixes.

## 0.7.1

* Typo fix, from persistance to persistence.

## 0.7.0

* Added persistance support
  [#36](https://github.com/mcollina/mosca/pull/36).
* Updated Ascoltatori to 0.7.0.

## 0.6.0

* Extracted a MoscaClient.

## 0.5.0

* Bunyan support for logging.
* Updated minimum MQTT.js version to 0.2.10.

## 0.4.3

* Passing the MQTT packet details to Ascoltatori
  [#30](https://github.com/mcollina/mosca/pull/30) by
  [@davedoesdev](https://github.com/davedoesdev).

## 0.4.2

* Not passing the options to subscribe anymore
  [@davedoesdev](https://github.com/davedoesdev).
* Updated Ascoltatori to 0.6.0.

## 0.4.1

* Fixed the NPM script.

## 0.4.0

* Pass the QoS level to the parent MQTT server
  (https://github.com/mcollina/mosca/pull/26), thanks to
  [@davedoesdev](https://github.com/davedoesdev).

## 0.3.0

* Node v0.10 support
* User authentication and authorization.

## 0.2.0

* QoS 1 (without storage) support
* Will messages support

## 0.1.1

* Bug fixes

## 0.1.0

* Initial release

