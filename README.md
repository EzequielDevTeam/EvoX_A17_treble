# EvoX A17 GSI Treble (pioneiro)

Evolution-X no **Android 17** (`cnb`) com o trio Doze-off pra GSI TrebleDroid. Ninguém fez ainda — esse repo é a tentativa, então espera poeira.

## O que tem aqui

- **ROM:** `Evolution-X/manifest` no `cnb` (A17)
- **Device tree:** `Doze-off/device_phh_treble-doze` (ainda no `android-16.0` — port pra A17 pendente, é o próximo trampo)
- **Overlays:** `Doze-off/vendor_hardware_overlay`
- **Treble app:** `Doze-off/treble_app-doze`

Manifest: `EvoX_A17.xml`.

## Build (na nuvem, nada no telefone)

Workflow `build-gsi.yml` (manual). Primeiro valida o sync + `lunch evox_gsi-userdebug`, depois vem o `mka`.

## Onde vai doer

1. Device tree A16 em base A17: sepolicy e API vão reclamar — port iterativo.
2. Sync full é pesado pro runner: se estourar disco, apara grupos e tenta de novo.
3. `TrebleApp.apk` prebuilt: confirmar a integração no primeiro build que passar.
4. Teste via DSU Sideloader antes de pensar em flash (ver README do Doze-off).

## Suporte

Grupo Doze-off: https://t.me/dozeoff_treble
