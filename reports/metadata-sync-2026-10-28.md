# Metadata Sync Receipt — October 28, 2026

## Scope

This batch adds missing YAML `description` metadata to the 23 source documents identified by the rendered Quarto verification report for `Feirbrand/synoeticos-public`. No other repository content was changed. The two Elevation Grid overlay files also had a legacy leading/inner blank-line issue that caused their existing YAML block to render as body text; only those delimiters were normalized so the new metadata is recognized by Quarto.

## Commit

| Repository | Commit | Message |
|---|---|---|
| `Feirbrand/synoeticos-public` | `3fd57298a12fef9e7d0b8c1d559c90143a27240c` | `docs: add missing Quarto meta descriptions` |

## File evidence

| Path | Git blob SHA-1 | SHA-256 content hash | Bytes |
|---|---|---|---:|
| `docs/cognitive-mage-v1.0/index.qmd` | `fba6865354e85d1baaa342dccb64873d28446ecc` | `596e2c38321c3c111d3eaecd0af9653b09eb647fed8f7b069ed9cbe765557d50` | 11,388 |
| `docs/developer-guide/index.md` | `4ac057bb49fd5bd741a97f706b97eb15c4cd9dc9` | `c0ae1844274f992ba73d92933aa2e819dddbe2f388efe84114f59a40b6b21518` | 3,247 |
| `docs/elevation-grid/elevation-grid-cross-references.md` | `14509fca66793b36880f077aaaf754c60d72cdfd` | `4e5057c98bd9ba1b134ae319a7cbf397fd5dde0fe511bad48900525bd5ab29e3` | 9,497 |
| `docs/elevation-grid/elevation-grid-cts-overlay.md` | `b1be5aeee91a70c1b0f2822fc4398cbaabb3514a` | `08e3d26827ac08663438781a0b85018fca9c4b40960433ba7b1f48bc6c19d2d2` | 17,364 |
| `docs/elevation-grid/elevation-grid-master-bibliography.md` | `296a02fdbbc990a9c4be9a1e385d117a57502c13` | `047408ad247f431b47789d93c3b34f46283dd5cb4f83062762e5acd2ed76c78f` | 9,778 |
| `docs/elevation-grid/elevation-grid-synoetic-overlay.md` | `7789889cb6057ecad49ca239e852098e78ccd628` | `dd7603e9fa83a9065d8544b81c8bc15ad05695f1879274ebd5e542a5cd7345fe` | 14,759 |
| `docs/elevation-grid/index.qmd` | `d3f3115ee1e96881468eb7f62309953faa0714e3` | `81ffde330e94012ade783e2cfe96e9a50901d43de03087ec754f70a6ec9acbc3` | 12,409 |
| `docs/fce-v3.6/fce-v3.6-cross-references.md` | `4a9fe20b216c5f6aa9a843a4156eb8de7d901b31` | `a3c5fe0b47f199c01edef52a9232ef069e94139a92742f5654820d5220c41070` | 4,337 |
| `docs/fce-v3.6/fce-v3.6-master-bibliography.md` | `e06c12704e69629de3b0f67e7774b3c29cc0eb87` | `e3171e3ddc269309b3d850d67a5fce66937aa1be2531dd29aa3fa5e3541dfeed` | 4,081 |
| `docs/fce-v3.6/index.qmd` | `af91b90e8db686035c80162dde0ebe7416ba9da6` | `0a41b918d2e9ac202813b354aa0435de9386a1b782b39bccf6451887c53519d` | 9,939 |
| `docs/index.qmd` | `01740da18da9dd0541a012ee089b35411cbde72a` | `6fcbc499fab1646ecac2128886d83210b23d3121366e0d07332309082e303b7c` | 12,585 |
| `docs/mi-agents-v1.0/index.qmd` | `0ea6d004edef39d85cf4d0d25516f4a0bf1f1ff7` | `d2d7eb7bb28a2f34593c9d3f71e150744ead16e6700b01bae1166ab1e8ad84eb` | 12,523 |
| `docs/neuroformation-v1.0/neuroformation-cross-references.qmd` | `b1f9bc97f43812bbeedd3a20f3cf01b4a44eaf4d` | `15d55d9ea757eff5380b4048632a9b48859d140a3064962832e7c9109c865acf` | 4,262 |
| `docs/neuroformation-v1.0/neuroformation-master-bibliography.qmd` | `365920024ce6def89e9a73e13a4e553ce0efac00` | `c31f4e1023ca7789fa4812748c6d7adf4dc31e9469b19603e1a5fde1f75e0b29` | 9,100 |
| `docs/neuroformation-v1.0/neuroformation-visualizations.qmd` | `2e66c17abf118e320faf1dfef1495f2c4badd1f5` | `9aa6b43b83746b2a1812bb727c8953be04f97fc55bbc735dc0697be09c377929` | 3,542 |
| `docs/pme-v1.0/index.qmd` | `053aeea66a50a86f8277cef5d866ba45964c8c4f` | `5060e70b9f7b5332b51fdf179132be3ce14a1f89d7cfdf857dd8a625d2464d42` | 10,825 |
| `docs/pme-v1.0/pme-v1.0-cross-references.md` | `fc301680ca99252675696964538a04c5d1045ae2` | `70712a17f28ccfdf71a2c108ce2d17ddc0060e156b85701c7e45969e44f71d36` | 12,517 |
| `docs/pme-v1.0/pme-v1.0-master-bibliography.md` | `3aee0019a87aded5c60e186f39e4bd96fdbcee07` | `f689b8b3518a1bf75e61e44b7f67ecec780818ef9df781b80a9ccbdfcb182c1d` | 15,194 |
| `docs/synoetic-os-v1.0/index.qmd` | `0a2c9dd7bdb9379e05fc84fbd391cda41c56af93` | `fad1d5620e06318f535a9079db64917e1e026b664b3aa1351c2e4c2bbe743af8` | 11,664 |
| `docs/torque-v2.0/index.qmd` | `b55b68cce492b804da826698905fd2023bccf292` | `eb775d9336db12ea16f27a3c187eaaea9d1ab0914ac4ef6c53f8c085da83351d` | 10,678 |
| `docs/utme-v1.0/index.qmd` | `8a0013c6168663b8a0abf98c695fd7e93c92a37a` | `95740f4cbfc219e87787e6cd45a984766517e794670154b16ba3a8554c4e3665` | 14,116 |
| `docs/utme-v1.0/utme-v1.0-cross-references.md` | `ea895aa6b2a6e9ea2681a96a72f6c13fd34975a9` | `b71e3e65712913c44e5bd045e95da10bbac8fde94a12c315aeb812e8133355f2` | 5,118 |
| `docs/utme-v1.0/utme-v1.0-master-bibliography.md` | `7497eb673a9d7aa926b9179842d1a7e0a9286a99` | `1c69166f112928142d1f6362a16e8348e896fa4dd79cd90bf75015b7ca36764c` | 7,745 |

## Verification

Quarto `1.8.0` rendered all 53 HTML documents successfully. The final rendered crawl found 2,658 internal path links with zero broken targets and 1,299 fragment links with zero broken anchors. All 53 pages have a `<title>` and all 53 pages now have a non-empty `<meta name="description">`. `git diff --check` passed.

The source working tree contains only the 23 intended metadata changes at this stage. No paper bodies, data values, citations, DOIs, or external records were changed.
