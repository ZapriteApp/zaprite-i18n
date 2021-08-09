# zaprite-i18n

![zaprite-i18n-earn-sats@2x](https://user-images.githubusercontent.com/12265052/128745690-bd37dd76-947b-4032-a1d0-ab01b33a70fd.png)

## Introduction

This repository includes all the strings used in the Zaprite web app (https://app.zaprite.com).

If you would like to translate a language, view the [Project board](https://github.com/ZapriteApp/zaprite-i18n/projects/1) and choose one of the languages in the _To do_ column. Then, reach out to us and let us know you would like to work on it.

If you don't see your preferred language anywhere on the Project board, [email us](mailto:support@zaprite.com) or reach out on [Twitter](https://twitter.com/ZapriteApp) and we will organize adding it to the project.

## Payment

1. We will pay USD$75 **in bitcoin** for each language translated.
2. You **must** send your invoice using Zaprite. 🙂

---

# How to translate

### IMPORTANT: Check the Project board first!!

https://github.com/ZapriteApp/zaprite-i18n/projects/1

If a language is _In Progress_ it means it has already been assigned. Please **do not** start working on a language that has already been assigned, or without getting the go-ahead from us first. **You will not get paid.**

### 1. Sign up for a Zaprite account

You will need a Zaprite account to invoice us, but it will also help to visualize where each string is located for better context.
https://app.zaprite.com

_Note: We only require an email and strong password to sign-up. No KYC!_

### 2. Get the language files

There are three ways you can work on translations:

1. Clone this repo, _or_
2. Download a copy of the JSON files for your assigned language from this repo.

### 3. Translate the strings

Use your favourite text editor to edit the files, which are all in JSON format.

Each file includes `"key": "value"` pairs. We require the `"value"` side to be translated.

#### Examples

File:
`tasks.json`

Sample snippet:

```json
{
	"list": {
		"page_title": "Tasks"
	}
}
```

In the above example, only the word `Tasks` needs to be translated, as it has a corresponding _key_ (`page_title`).

The screenshot below is another example that shows the highlighted strings that need to be translated …

![tasks_json_example](https://user-images.githubusercontent.com/12265052/124162027-eb03cb80-da52-11eb-9b7d-d3f1f9cf4b2a.png)

#### HTML Strings

You may see some strings that contain HTML wrapper tags. For example:

```json
"modal": {
    "warn": "<0>You <1>cannot undo</1> this action!</0>"
}
```

All the HTML wrapper tags (`<0>, <1>, <2>, …`) must be kept. However, they may need to be moved depending on the language being translated. You can always ignore the `<0>` tags, as these just reference the overall string wrapper, and will remain at each end of the string. You only need to account for all tags from `<1>` and up.

In the simple example above, the `<1></1>` tags refer to **bold** text, highlighting an important part of the message.

If you were translating into Spanish, for example, you might translate that string as follows:

`<0>¡No <1>puede deshacer</1> esta acción!</0>`

In German, however, you might need to move the tags:

`<0>Diese Aktion <1>kann nicht rückgängig gemacht werden!</1></0>`

Please use your best judgement and try to make sure the HTML wrappers are around the same context. This may be tricky where multiple HTML tags are present.

> Feel free to reach out using the contact info below if you are unsure about any string.

#### Variables

You may also see some strings that contain variables, or a mix of variables and HTML tags. For example:

```json
"verify": {
    "confirm": "<0>We have sent a verification email to <1>{{email}}</1></0>"
}
```

You _do not_ need to translate the variable text inside the double curly brackets. In the example above, the word `{{email}}` **does not** need to be translated.

Again, just make sure the variables and brackets (`{{variable}}`) stay in the translation in the correct place.

### 4. Submit the translations

If you use Github, you can create a pull request with your changes included.

Alternatively, you can email the updated JSON files to [support@zaprite.com](mailto:support@zaprite.com).

### 5. Send your invoice

If everything looks good we will let you know and you can then send your invoice using Zaprite.

---

# Some tips!

Sign up for a Zaprite account before you start translating. You will be able to browse through the app and visually see where each string is located to get better context for how the wording is used.

You also need a Zaprite account in order to invoice us for your work, so it would be more beneficial to sign-up before you begin. 👍

# Questions?

If you have any questions:

1. Reach out on Twitter [@ZapriteApp](https://twitter.com/ZapriteApp), or
2. Email us at [support@zaprite.com](mailto:support@zaprite.com)

Cheers!
