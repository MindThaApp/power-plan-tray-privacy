# Power Plan Manager privacy policy

Last updated: 30 October 2026

Power Plan Manager (Pro and Lite editions) is a Windows power-plan and battery-care app, made by MindtheApp. This page explains, in plain words, what the app does with your information. The short version: it does not collect usage data, analytics or telemetry, has no accounts and no advertising, and does not require an internet connection. The only information that can leave your PC for us is a crash report (only with your consent) or a feedback message you choose to send, as described below.

## Crash reports

When Power Plan Manager crashes or stops responding, it can send us a crash report: the type of error and its message (or, for a crash inside Windows components, the error code and the component's name), the list of program functions that were running (the stack trace), how long the app stopped responding, the app version and edition, the Windows version and language, and basic device facts such as the processor type. Before anything leaves your PC, file and folder paths are reduced to placeholders (for example `%USERPROFILE%\Documents\<file>.txt`), your user name and your PC's name are removed, and so are network details such as IP addresses, web addresses, device names on your network, e-mail addresses and anything that looks like a password or token. No IP address is stored with a report, and no location is worked out from one. No files, screenshots or memory dumps are sent. Nothing is sent without your consent: by default, the app asks after a crash, and the report stays on your PC until you choose Send. You can choose "Send automatically" or "Never send" at any time in About > Crash reports; Never turns crash reporting off completely and deletes any report still waiting. With "Send automatically", the app also sends a small session record when it starts and ends (the app version and whether the session ended normally or in a crash, with no content), so we can see how often a version crashes. If you press "Send report", the same kind of redacted information is sent together with the app's crash, error and hang logs, the end of its tray log, the sensor helper's crash files and the app's settings, with all paths, names and network details removed. The passwords and tokens of smart plugs and Home Assistant are kept in the Windows credential store and are never part of a report. "Email instead" only saves the report to your Downloads folder and opens a draft in your email app; nothing is sent unless you send that email yourself. Reports are processed for us by Sentry (Functional Software, Inc.) and stored in its EU data region (Germany). A random installation number groups reports from the same copy of the app; it cannot identify you. Reports are kept for the retention period of our Sentry plan and are then deleted automatically. Reports are not linked to your identity, are not used for advertising or tracking, and are not sold or shared with anyone else. To ask about or delete a report, contact us and quote the reference shown after sending.

Crash reports also stay on your PC, in the app's local cache folder (the newest 20), until you clear them in About > Crash reports. With "Keep crash dumps on this PC" on (the default), the app also keeps a memory dump of its last five crashes or hangs there. A dump is never sent to Sentry; it is added only to a report you e-mail yourself, and you can delete it from the zip first. A dump can hold anything the app had in memory, so don't send one from a work or school PC that your organisation manages.

## Feedback

In About > Send feedback you can send us a message. Only when you press Send, the text you wrote, the type you chose (question, idea, problem, praise or other), the app version and edition and, if you typed one, your email address are sent to Sentry (Functional Software, Inc.), which processes them for us in its EU data region (Germany). Before the message leaves your PC, file and folder paths, your user name, your PC's name and network details such as IP addresses are replaced in your text. No IP address is stored. Your email address is optional and is used only to reply to you; it is not used for anything else. If you tick "Include a diagnostics report" (off by default), the same redacted diagnostics as "Send report" are attached. Sending feedback does not depend on the crash-report setting, because pressing Send is your decision, and nothing else is sent. If a message cannot be delivered, the app says why and offers an email draft instead; a message that was not delivered may be retried on a later start. To ask about or delete a message, contact us and quote the reference shown after sending.

## Data that stays on your PC

Preferences, automation rules, schedules, presets, and the power, energy and battery history are stored locally in the app's Windows application-data folder. Exported profiles and reports are written only to a file or folder you choose.

If you add a smart plug or energy meter (for example Shelly, Tapo, Kasa, Tasmota or Home Assistant), the app reads its power readings directly over your local network from the address you enter. The plug's password or access token is kept in the Windows Credential Locker on your PC. These readings are not sent to us or anyone else.

## Administrator rights

The app normally runs without administrator privileges. Windows shows a User Account Control prompt only for actions you start:

- a narrowly scoped `powercfg` operation when you create or remove standard power plans or change the visibility of advanced power settings;
- the optional sensor helper, a small program inside the app package that reads hardware sensors (CPU power and temperature, motherboard and fan sensors) and, when you ask, controls fan speeds. It uses the open-source LibreHardwareMonitor library and the signed PawnIO driver, which the app installs through Windows Package Manager only after you confirm. If you turn on "Start sensor helper with Windows" or "Start fan control when the PC starts", the app registers a Windows scheduled task for it; turning the option off removes the task. The helper keeps its log, crash files and saved fan settings in `%ProgramData%\PowerPlanManager\SensorHost` and talks only to the app on your PC.

Only these operations are elevated; the app itself is not restarted or kept running as administrator.

Power Plan Manager reads and changes local Windows power-plan, battery and fan settings solely to provide the features you request. It does not send those settings anywhere.

## Purchases

Power Plan Manager's optional Pro features (in the free edition) or Pro app and its add-on are purchased through the Microsoft Store. Microsoft handles all payment details; the app only learns whether you own a licence, never your payment information.

## Children

Power Plan Manager is not aimed at children and does not knowingly collect personal information from them. The only personal information it can send is an e-mail address someone chooses to add to a feedback message.

## Changes

If this policy changes, the updated policy will be published on this page.

## Contact

Questions about this policy, or to ask about or delete a report or message: mindthaapp@gmail.com
