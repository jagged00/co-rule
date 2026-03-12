# Christian Queen Co-Ruler (CK3 Mod)

This mod gives Christian female rulers a "co-ruler" style marriage outcome:

- When a Christian female ruler marries an adult male spouse, her husband receives a permanent **Co-Ruling Husband** modifier.
- The wife receives a small "shared rule" prestige/vassal bonus.
- The husband is set as designated regent when possible, so he is mechanically recognized in governance.

## Files

- `common/on_action/co_rule_on_actions.txt` hooks into `on_marriage`.
- `events/co_rule_events.txt` applies the co-rule effects.
- `common/modifiers/co_rule_modifiers.txt` defines bonuses.
- `localization/english/co_rule_l_english.yml` provides English localization.

## Notes

- In vanilla CK3 there is no universal hard "co-ruler" title for all governments, so this mod models co-rule using modifiers + designated regency.
- If you use a custom government that supports a specific co-monarch command, you can extend `co_rule.0001` with that effect.
