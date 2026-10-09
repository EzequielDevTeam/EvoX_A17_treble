# EvoX A17 GSI Treble (pioneiro)

Evolution-X base **Android 17** (`cnb`, `android-17.0.0_r1`) + trio Doze-off, para GSI TrebleDroid. Ninguém fez ainda — este repo é a tentativa.

## Base

| Parte | Origem | Branch |
|---|---|---|
| Manifest/ROM | `Evolution-X/manifest` | `cnb` (A17) |
| Device tree | `Doze-off/device_phh_treble-doze` | `android-16.0` (⚠️ port p/ A17 pendente) |
| Overlays | `Doze-off/vendor_hardware_overlay` | `pie` |
| Treble app | `Doze-off/treble_app-doze` | `master` |

Manifest: `EvoX_A17.xml` (EvoX cnb + trio).

## Build (nuvem, nunca no telefone)

Workflow `build-gsi.yml` (manual). v1 = probe de sync + `lunch evox_gsi-userdebug`. Sem nada baixado no telefone.

## Riscos conhecidos

1. Device tree A16 sobre base A17: esperar erros de sepolicy/API — port iterativo.
2. Sync full AOSP pode estourar disco do runner — v2 apara grupos se precisar.
3. Integração do `TrebleApp.apk` prebuilt a confirmar no primeiro build.
4. Teste via DSU Sideloader antes de flash (ver README Doze-off).

## Suporte

Grupo Doze-off: https://t.me/dozeoff_treble
