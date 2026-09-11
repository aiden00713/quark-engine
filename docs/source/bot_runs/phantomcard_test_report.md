# PhantomCard groundtruth test (bot)

Family: PhantomCard (NFC relay / card-skimming Android malware).
Validated against upstream human Quark rules #247–#251.

## Detection on samples
- Samples tested: 9 (1 hash not found on MalwareBazaar)
- Quark with full old_rules: **9/9 High Risk**
- Quark with #247–#251 only: all samples matched the five human rules

## Bot RuleForge generation vs human #247–#251
- Bot generated rules: 418
- Accuracy (recall vs human 5 rules): **40%**
- Precision: **N/A** (no benign control set)
- Matched: #250, #251
- Missed exact pairs: #247, #248, #249

## Tested APKs
| SHA256 | Source | Risk level |
|--------|--------|------------|
| `0d5fd1997ecb76a167df753d5cce7688dfd0d813c028c9644025da352af77b7d` | MalwareBazaar | High Risk |
| `21c66fe505f2bcd7b29d413189920b3a85df48da0ecf4eb6962d6a504a7fdcd8` | MalwareBazaar | High Risk |
| `2922fcf373e2caf3588266cfafeaafbc74304c81d024315d279f0ea537adc1b6` | MalwareBazaar | High Risk |
| `360966ad8752d040e9aaae5cb4a5913e6f85edcf56ecfeb8246729b45d0e6c78` | MalwareBazaar | High Risk |
| `a78ab0c38fc97406727e48f0eb5a803b1edb9da4a39e613f013b3c5b4736262f` | MalwareBazaar | High Risk |
| `ab2906d88e4f64ec0784ef8fdf132bb7ca9a914c037c3b731803f3adfd7a8f66` | MalwareBazaar | High Risk |
| `cb10953f39723427d697d06550fae2a330d7fff8fc42e034821e4a4c55f5a667` | MalwareBazaar | High Risk |
| `d3f863757e946d117ee7c7b50e480264a2ff1a08e7925bd2de3e6c43182868ed` | MalwareBazaar | High Risk |
| `e27579b92fcad2f4fe96db7b5e7a7cdc41754a7cd126fcaf598d3f8d8c21c0f5` | MalwareBazaar | High Risk |

## Notes
- Workflow test for quark-rule-forge. Samples deleted after the run.
- Requires human review before merge.
