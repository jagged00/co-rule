# Christian Queen Co-Ruler (CK3 Mod)

This mod gives Christian female rulers a "co-ruler" style marriage outcome:

- When a Christian female ruler marries an adult male spouse, her husband receives a permanent **Co-Ruling Husband** modifier.
- The wife receives a small "shared rule" prestige/vassal bonus.
- The husband is set as designated regent when possible, so he is mechanically recognized in governance.

## Files

- `common/on_action/co_rule_on_actions.txt` hooks into `on_marriage` and includes a yearly compatibility backfill.
- `events/co_rule_events.txt` applies and maintains the co-rule effects.
- `common/modifiers/co_rule_modifiers.txt` defines bonuses.
- `localization/english/co_rule_l_english.yml` provides English localization.

## Save Compatibility

- A yearly pulse (`on_yearly_pulse`) checks living characters and applies co-rule effects to Christian female rulers with eligible husbands.
- The yearly check is filtered so it only triggers for rulers still missing one of the co-rule modifiers.
- This ensures existing saves started before installing the mod are brought up to date over time.

## Byzantine / Administrative Co-Ruler Mechanic

- You can absolutely roleplay this in Administrative/Byzantine campaigns, but CK3 scripting does **not** expose one universal, cross-government script effect that reliably grants the government-specific co-ruler office in all contexts.
- Because of that, this mod uses mechanics that always exist (modifiers + designated regency), so it remains stable across governments and save states.
- If your setup uses a known scriptable Administrative co-ruler command from another mod/framework, add it inside `co_rule.0001` before the regency fallback.

## Notes

- In vanilla CK3 there is no universal hard "co-ruler" title for all governments, so this mod models co-rule using modifiers + designated regency.
