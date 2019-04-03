# Nova Extension: Dynamic Policies

This extension replaces the standard Nova policy page with one that will list both the default policies as well as any additional policies a sim defines within its `Site Messages`.

## Requirements

This extension requires:

- Nova 2.6+

## Installation

Copy the entire directory into `applications/extensions/dynamic_policies`.

Add the following to `application/config/extensions.php`:

```
$config['extensions']['enabled'][] = 'dynamic_policies';
```

## Usage

To define a policy in addition to the default policies, go to `Site Management > Messages and Titles` and then `Add New Message`. For the new message, give it a message key of `policy-whatever`, where `whatever` is a unique name for the policy you're adding. Then, when you go to `Site Policies` (aka. `main/policies`), it will now show up in the list of policies.

To define a message that shows up introducing your policies, you can also add a message with a message key of `policies`. This will show up before the list of policies on this dynamic policies page.

## Issues

If you encounter a bug or have a feature request, please report it on GitHub in the issue tracker here: https://github.com/jonmatterson/nova-ext-dynamic_policies/issues

## License

Copyright (c) 2019 Jon Matterson.

This module is open-source software licensed under the **MIT License**. The full text of the license may be found in the `LICENSE` file.
