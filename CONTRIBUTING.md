# Contributing to Cosmiq

Thanks for helping improve Cosmiq. Bug reports, suggestions and translations from the community help us a lot.

We read every issue, but it takes time, especially when issues are duplicates or are missing information. Please read this whole page before you open an issue or pull request.

> [!TIP]
> Don't open an issue to ask a question or to get help. Ask in the Cosmiq Discord instead. You can find the invite in the [README](README.md).

> [!IMPORTANT]
> Don't report security vulnerabilities, account problems or payment problems in a public issue. Contact the Cosmiq team privately through the Discord or the [website](https://cosmiq.gg).

## Bug reports

1. **Search first.** Check [open and closed issues](../../issues?q=is%3Aissue) to see if the bug has already been reported or fixed.
2. **Update first.** Make sure you're using the latest version of Cosmiq for your Minecraft version. The bug may already be fixed.
3. **One bug per issue.** If you found several bugs, open a separate issue for each.
4. **Use the [bug report template](../../issues/new?template=bug_report.yml)** and fill in every required field.

A good bug report includes:

- **Clear steps to reproduce the bug.** If we can't reproduce it, we probably can't fix it.
- **Your logs.** Upload `latest.log` from `.minecraft/logs` to [mclo.gs](https://mclo.gs) or a GitHub Gist, and paste the link. If the game crashed, also include the crash report from `.minecraft/crash-reports`. **Crash reports without a crash log will be closed.**
- **Your mod list,** if you have other mods installed. If Cosmiq is the only mod you use (other than Fabric API or your loader's required mods), write `None`.
- **Screenshots or videos,** if they help show the problem.

> [!TIP]
> To check whether another mod causes the bug, try reproducing it with only Cosmiq and its required dependencies installed.

## Suggestions and feature requests

We get lots of suggestions and can't add all of them. We may close a suggestion if it doesn't fit Cosmiq, is too difficult to add, or has already been suggested.

1. **Search first.** Check [existing issues](../../issues?q=is%3Aissue) for the same idea. If you find it, add a 👍 reaction instead of opening a new issue.
2. **One suggestion per issue.**
3. **Use the [feature request template](../../issues/new?template=feature_request.yml)** and explain what you want and why.

> [!WARNING]
> **Please don't suggest:**
> - Support for a specific Minecraft version or loader. We'll add versions when we can.
> - Specific cosmetics. Cosmetics are created and released through Cosmiq, not through GitHub issues.
> - Features that we've already announced or shown.

## Translations

Translations are in the [`lang/`](lang) folder. `en_us.json` is the source file. It always has the newest keys and English text.

### Add or update a translation

1. **Fork** this repository.
2. **Copy** `lang/en_us.json` to a new file named with your [Minecraft language code](https://minecraft.wiki/w/Language#Languages), such as `de_de.json`, `fr_fr.json` or `pt_br.json`. If the file already exists, edit it instead.
3. **Translate the values only.** Don't change the keys, which are the text on the left of the `:`.
4. Open a **pull request** with a title like `Translation: German (de_de)`.

```json
{
  "key.cosmiq.emote_wheel": "Emote-Rad"
}
```

### Translation rules

- **Keep placeholders.** Keep `%s`, `%1$s`, `%d` and similar codes in your translation. You can move them in the sentence, but you can't remove them.
- **Keep the file valid JSON.** Use double quotes, put commas between entries and don't add a comma after the last entry. If you aren't sure, check the file with a JSON validator.
- **Save the file as UTF-8.**
- **Keep it short.** Some text appears on buttons and in small menus, so try to keep translations about as long as the English text.
- **Translate by hand.** Don't submit raw machine translations. You can use a translator as a starting point, but check the result yourself.
- **Keep "Cosmiq" as it is.** Don't translate the product name.
- **One language per pull request.**

When we add new English text, untranslated keys will show in English until someone translates them. You're welcome to open a pull request that adds the missing keys to an existing language.

## Pull requests

Pull requests here should only change files in `lang/` or fix mistakes in the documentation. Cosmiq's source code isn't in this repository, so we can't accept code changes here.

By submitting a contribution, you agree that it's covered by section 3 of the [LICENSE](LICENSE).

## Conduct

Be respectful. We'll close or lock issues and pull requests that contain harassment, spam or abusive language, and we may block the people who post them.
