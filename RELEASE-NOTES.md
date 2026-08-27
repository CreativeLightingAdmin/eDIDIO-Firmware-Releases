# eDIDIO Firmware Release Notes

## 1.5.6

* Fixed an issue where the device could restart when queried by a BACnet client.
* Fixed an issue where the BACnet BBMD broadcast distribution table was not retained after a restart.

## 1.5.5

* Fixed an issue where device discovery reported TLS even when the device was set to TCP only.

## 1.5.4

* Fixed an issue where DMX outputs could show incorrect levels at start-up on Art-Net and sACN systems.
* Firmware updates now transfer around 10% faster.

## 1.5.3

* Improved fault diagnostics available to support.
* Fixed an issue where deep, dim mixed colours rendered slightly off in Spektra.

## 1.5.2

* Added support for the V3 encrypted firmware format on provisioned devices.

## 1.5.1

* Embedded the production certificate authority used for secure device provisioning.

## 1.5.0

* Fixed an issue that could cause a firmware update to fail to apply.
* Faster firmware verification.

## 1.4.2

* More detailed feedback during a firmware apply.

## 1.4.1

* Live sensor status is returned in pages, reducing memory use on the controller.

## 1.4.0

* New live event and log stream with typed events.
* Live events now include sensor and DALI input line and address details.
* Requires an updated SpektraPlus to view live events.

## 1.3.3

* Sensor status now reports the device light setpoint and the group mean light level.
* Fixed an issue where an unresponsive sensor could hold a stale reading in the group average.
* Duplicate sensor addresses are rejected when sensors are programmed.

## 1.3.2

* Cooperative sensor group roles are named Leader and Follower to match the app.

## 1.3.1

* Sensor programming rejections now report the specific reason.

## 1.3.0

* New directional sensor grouping with Leader and Follower roles.
* All 40 sensors can now take part in cooperative groups.
* Requires an updated SpektraPlus, and sensors must be pushed again after updating.

## 1.2.4

* Fixed an issue where DALI-2 sensors could stop responding to motion after a power cycle.
* DALI-2 sensors are now configured once they are ready at start-up.

## 1.2.3

* Sensor status now indicates when a daylight-harvesting reading is still settling.

## 1.2.2

* Fixed an issue where lights could remain on in a cooperative sensor group.
* Fixed an issue where a grouped zone could stay off while the area was occupied.
* Fixed a brief light level jump when the regulating sensor in a group changed.

## 1.2.0

* Added SD card support for 6 Pole devices.
* Internal memory improvements.

## 1.1.6

* Fix for DMX properties.

## 1.1.5

* The bootloader version is now reported. Requires the latest bootloader.
* Fixed an issue where translations were not restored to defaults after a reset.

## 1.1.4

* DMX broadcast triggers now support zone control.

## 1.1.3

* Added next, previous and resume for sequences and themes.

## 1.1.2

* Added DMX properties.
* Added a sensor query command.

## 1.1.1

* Rewritten DALI transmit and receive.
* DALI transmit now supports collision detection and recovery.
* Added a send-twice option for DALI messages.
* Added support for data aliases.

## 1.1.0

* Internal memory allocation improvements.

## 1.0.86

* Improved log file handling.

## 1.0.85

* Fixed an issue where a DALI sensor could remain in a movement-detected state.
* Sensors are now configured at start-up.

## 1.0.84

* Fix for Spektra live data.

## 1.0.83

* Fixed an issue affecting the device after an SRAM battery replacement.

## 1.0.82

* Improved MAC address validation.

## 1.0.81

* Fix for Spektra theme validation.

## 1.0.80

* Spektra validation improvements.

## 1.0.79

* Spektra random background now uses the background colour.
* Fixed an issue with Spektra radial sequences running on a single fixture.

## 1.0.78

* Added firmware update commands.
* Added Spektra calendar defaults for theme and show.

## 1.0.77

* Added Spektra DT8 support for RGBWAF and XY.
* Fixed an issue where trigger commands could not target All Sensors.

## 1.0.76

* Improvements to lists and shows.
* Fixed daylight savings handling for UK and US locations.

## 1.0.75

* Added further list stop commands for Spektra Pro.
* Lists now support both Show and Normal types.

## 1.0.74

* Fixed an issue where lists could stop unexpectedly with Spektra Pro.

## 1.0.73

* Improved network packet handling.

## 1.0.72

* Merged the Spektra feature set into the main release.

## 1.0.71

* Fixed an issue where the DMX output could stop after an RDM exchange.

## 1.0.70

* Spektra improvements, including background colour.

## 1.0.69

* Added new Spektra sequence types.

## 1.0.68

* Fixed an issue where running a looped list could restart the controller.

## 1.0.67

* RDM improvements.

## 1.0.66

* DMX and RDM get and set fixes.
* DALI type 8 optimisations.
* Fix for network properties.

## 1.0.65

* Multicast re-enabled for SDDP.
* SDDP now identifies on a change of IP address.
* Improved network socket stability.

## 1.0.63

* The Ethernet link defaults to 10BASE-T, with auto-negotiation available from the
  on-screen menu.

## 1.0.62

* Added an option to select 10BASE-T or auto-negotiation for the Ethernet link.

## 1.0.61

* Improved DALI-2 addressing.

## 1.0.60

* Fixed an issue affecting compatibility with Sunricher drivers.

## 1.0.59

* Fix for SDDP device discovery.

## 1.0.58

* Fixed an issue where the controller could stop responding on networks with heavy multicast traffic.

## 1.0.57

* Fix for DALI addressing.
* Improved memory management.

## 1.0.56

* Fixed an issue where a momentary input could remain held after being disabled.
* Added a safety check for profile selection.

## 1.0.55

* Added the Spektra Intensity trigger type.

## 1.0.54

* Fixed an issue where subnet and DNS settings were not applied when set remotely.
* Improvements to logic actions.

## 1.0.53

* Added Identify Sensor as a network command.
* Improved stability of 24-bit DALI commands with a reply.

## 1.0.52

* Sensor initialisation now runs after sensors are programmed or the DALI type changes.
* Added mute and unmute sensor trigger commands.

## 1.0.51

* Added read-out protection support, not enabled by default.
* Added an Installation Tools menu with Passive Mode.

## 1.0.50

* Added the DALI multi-type query.

## 1.0.49

* SDDP updates to suit the Control4 driver.
* Added handling for the DALI type 8 RGBWAF command.

## 1.0.48

* Improved DALI event handling.

## 1.0.47

* RDM timing aligned to specification.

## 1.0.46

* RDM improvements for 4-pole.
* Added output state to device state reporting.
* Added a feedback system for triggers.

## 1.0.45

* Maintenance release.

## 1.0.44

* Memory and performance improvements for TLS.

## 1.0.43

* Memory improvements.

## 1.0.42

* Added a custom DALI type 8 XY command.
* The selected profile is included in system diagnostics.

## 1.0.41

* Updated internal DALI line ordering. No change to how the device is used.
* Fix for the Count Devices menu function on 9-pole.
* Improved progress feedback for Address New and Readdress All.

## 1.0.40

* Fixed an issue where the controller could fail to establish a network link after being plugged in.

## 1.0.39

* Improved DALI type 8 query responses.
* Added DALI type 8 store feature status.

## 1.0.38

* Refined the DALI type 8 CCT command.

## 1.0.37

* Added TLS support.

## 1.0.36

* Improved DALI event decoding.
* Added a higher level trigger event.
* Added a firmware verification checksum.
* Fixed an issue where fading DMX channels could output an incorrect level at start-up.

## 1.0.35

* DALI event messages now decode special commands.
* Improved DALI type 8 network queries.

## 1.0.34

* Updated the Control4 driver name.

## 1.0.33

* Updated the network stack in preparation for TLS 1.2.

## 1.0.32

* Fixes for DALI device type 2, RDM and DMX persistence.
* This version requires the EEPROM to be cleared.

## 1.0.31

* Improved accuracy of the device system logs.
* Logs are cleared when logging is first enabled from the keypad menu.
* Improvements to the screensaver and display dimming.

## 1.0.30

* Fixed an issue where DMX was not recognised by connected devices.
* Updated the reported hardware version to match the board.

## 1.0.29

* Added event filtering.

## 1.0.28

* Fixed an issue where an alarm could restart the controller.

## 1.0.27

* Improved event handling.
* DALI events now report packets received from other controllers.

## 1.0.26

* Improved trigger handling.
* Fixed an issue where sensors in one profile were marked unprogrammed after programming another.

## 1.0.25

* Added raw frame data handling for DALI messages.
* Added DALI commissioning commands.

## 1.0.24

* Added system logging, off by default, with selectable levels.
* Logging can be enabled by trigger or from the keypad.

## 1.0.23

* Added zone scaling for Spektra.

## 1.0.22

* Added a device reboot command.

## 1.0.21

* Added DMX fade zone commands.

## 1.0.20

* Improved 24-bit DALI sensor handling.

## 1.0.19

* Rewritten alarms, supporting repeat triggering and multiple alarms at the same time.
* A dedicated midnight alarm is no longer required.
* Rewritten daylight savings handling, including astronomical alarms.
* Rewritten DALI receive for 8, 16 and 24-bit frames.
* Improved DALI transmit timing for wider device compatibility.
* Added a screensaver option.
* Added validation for looping lists.

## 1.0.18

* Improved completeness of Read from Device, including the calendar overview.

## 1.0.17

* Increased the maximum number of Spektra zones to 10. Requires Spektra X 2.5.3 or newer.

## 1.0.16

* Added support for DALI-2 input devices, including switches and rotaries.
* Added Spektra sequence arguments, such as comet background colour and tail length.

## 1.0.15

* Added sensor trigger actions.

## 1.0.14

* Improved GPIO setup for 4-pole and 9-pole.
* Fixed an issue with 9-pole output and configuration indexing.

## 1.0.13

* Added device state reporting.

## 1.0.12

* The Spektra calendar now supports leap years.

## 1.0.11

* Added a first pass of DALI to DMX translation, not enabled by default.
* Improved admin message handling and validation.

## 1.0.10

* Improved time offsets for astronomical alarms.
* Fixed an issue with DALI group mapping sent from Spektra X.

## 1.0.9

* Spektra now supports up to 10 channels per colour.
* The maximum number of colours per theme or sequence is 20.

## 1.0.8

* Stop Sequence now also turns the lights off.
* Improved DALI line targeting.

## 1.0.7

* Fixed an issue where outputs were not remembered after a power cycle.
* Reworked outputs configuration and handling.
* Added 9-pole outputs support.

## 1.0.6

* Improved sensor and burn-in handling before DALI frames are sent.
* Added unscheduled day behaviour for the Spektra calendar.
* Added Tridonic MSensor light harvesting.

## 1.0.5

* Added random colour order for Spektra sequences.

## 1.0.4

* Added extended lists, up to 32 lists with 256 steps each.

## 1.0.3

* Added support for long DMX fades.
* Increased the maximum colours per sequence or theme to 32.

## 1.0.2

* Removed the minimum step time on sequences.
* Fixed an issue where colours could stay on during sequences with a large number of fixtures.

## 1.0.1

* Alarms support month and weekday scheduling.
* Alarms support separate start and end triggers.

## 1.0.0

* Initial release.
