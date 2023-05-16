# austerity
You lack discipline! It's ok, though. This is like having discipline.

This package attempts to use every Dart and Flutter code rule available that doesn't cause major headaches, is not incompatible with other rules, and turns the error severity up to error. That means the code will display errors when you do something wrong. Use this package to get the strongest warnings about code violations, and use `analysis_options.yaml` to dial it back when you need to.

This is what you will see when you do naughty things
![errors](https://github.com/MelbourneDeveloper/austerity/blob/main/doc/images/errors.png) 

This library is pretty stable now. This will probably be the last beta version. 

## Dart 3 Upgrade!

austerity 1.1 removes options that were deprecated in Dart 3 and adds all these new lints!

Check it out! It's now even more austere!

- collection_methods_unrelated_type
- combinators_ordering
- dangling_library_doc_comments
- deprecated_member_use_from_same_package
- implicit_call_tearoffs
- implicit_reopen
- invalid_case_patterns
- matching_super_parameters
- no_literal_bool_comparisons
- type_literal_in_constant_pattern
- unnecessary_breaks
- unnecessary_library_directive
- unreachable_from_main
- use_string_in_part_of_directives

## Use the package
- Install the package in the `pubspec.yaml`
- Add this line at the top of your `analysis_options.yaml`

```yaml
include: package:austerity/analysis_options.yaml
```

## Configure Rules
You can easily turn the rules off or change the severity to warning. I dialed down a couple of rules due to personal preference, but you can see all of these in the [comments](https://github.com/MelbourneDeveloper/austerity/blob/main/lib/analysis_options.yaml) and adjust these for yourself. You have to understand that there are two types of settings: linters and analyzer rules. Most analyzer rules have a corresponding linter. You can remove the linter or change the severity of the analyzer rule. See the official documentation [here](https://dart.dev/guides/language/analysis-options).

![errors](https://github.com/MelbourneDeveloper/austerity/blob/main/doc/images/config.png) 

## Avoiding Breaking Changes
These analysis options change regularly. If new linters appear for the language, they will appear here and break your code. To avoid this, use a specific version of this package. 

✔️ Stable
`austerity: 0.0.8-beta`

❌ Potential Breaking Changes
`austerity: ^0.0.8-beta`