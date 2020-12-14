# i18n definitions

## Quickstart
For the localization [jQuery.i18n](https://github.com/wikimedia/jquery.i18n) is used.

For the following languages you need to import the language function script:
```
- Bosnian (bosanski)
- Lower Sorbian (Dolnoserbski)
- Finnish (Suomi)
- Irish (Gaeilge)
- Hebrew
- Upper Sorbian (Hornjoserbsce)
- Hungarian
- Armenian
- Latin (lingua Latina)
- Malayalam
- Ossetian
- Russian
- Slovenian (Slovenšcina)
- Ukrainian
```
These are located in `vendors/jquery.i18n/languages`

## Message Keys
The translation keys will be as follows:
```
DIRECTORY.(DIRECTORY.)FILENAME.ID.PLACE
```
For example for alerts:
```javascript
$.append(helpers.getDropdownGroup('follow-toggle', 'Enable Follow Alerts', (e.followToggle === 'true' ? 'Yes' : 'No'), ['Yes', 'No'],
                'If a message should be said in the channel when someone follows. This also toggles the reward.'))
```
so for this the message key should be:
```
alerts.alerts.follow-toggle.title
```

If needed put before or after the `ID` another describing word.

The only exception to this rule is the main.json there the message key starts with `main.`