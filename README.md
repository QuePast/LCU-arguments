# Riot Client / LCU Launch Arguments

A comprehensive reference of command-line flags accepted by the Riot Client and League Client Update (LCU) executables.
---

## Table of Contents

- [RiotClientServices.exe — Riot-specific flags](#riotclientservicesexe--riot-specific-flags)
- [Riot Client.exe — Chromium / Node.js / V8 flags](#riot-clientexe--chromium--nodejs--v8-flags)
- [CEF / Chromium highlights](#cef--chromium-highlights)

---

## RiotClientServices.exe — Riot-specific flags

| Argument | Value | What it does | Example | Notes |
|:---|:---:|:---|:---|:---|
| --agent | String | | | |
| --agent-auth-token | String | | | |
| --agent-bootstrap | | | | |
| --agent-check-installs | | | | |
| --agent-pid | Integer | | | |
| --agent-port | Integer | | | |
| --agent-prepare-directory | | | | |
| --allow-multiple-clients | | Allows multiple client instances; also disables patching |  | |
| --analytics-collector-url | String | | | |
| --app-command | String | | | |
| --app-listen-address | String | | | |
| --app-name | String | | `--app-name=""` | |
| --app-pid | Integer | | | |
| --app-port | Integer | | `--app-port=12345` | |
| --app-root | String | | | |
| --attach-session-pid | Integer | | | |
| --auto-kill | | | | |
| --automation | | | | |
| --auto-show | | | | |
| --ccs | | | | |
| --client-config-cooldown-period-secs | Integer | | | |
| --client-config-local-file | String | | | |
| --client-config-override-file | String | | | |
| --client-config-readonly | | | | |
| --client-config-url | String | | `--client-config-url=https://clientconfig.rpg.riotgames.com` | |
| --client-user-data-root | String | | | |
| --connect | | | | |
| --crashpad-environment | String | | | |
| --credentials-file | String | | | |
| --data-root | String | | | |
| --debug-break | | | | |
| --developer-force-external | | | | |
| --developer-patchline | String | | | |
| --developer-pid | Integer | | | |
| --developer-product | String | | | |
| --developer-version | String | | | |
| --device-scale-factor | Float | | | |
| --disable-auto-launch | | | | |
| --disable-auto-size-clamping | | | | |
| --disable-crashpad | | Disables crash reporting | `--disable-crashpad` | |
| --disable-elevation | | | | |
| --disable-launch-agent | | | | |
| --disable-manifest-verification | | | | |
| --disable-multirange-requests | | | | |
| --disable-patching | | Skips patching on launch | `--disable-patching` | |
| --disable-run-in-background | | | | |
| --disable-self-update | | Skips self-update check | `--disable-self-update` | |
| --disable-telemetry | | Disables telemetry collection | `--disable-telemetry` | |
| --dradis-endpoint | String | | | |
| --enable-run-in-background | | | | |
| --entitlements-url | String | | | |
| --env | String | | | |
| --environment-none | | | | |
| --fail-install | | Testing flag: forces install failure | | |
| --fail-launched-update | | Testing flag | | |
| --fail-new-update | | Testing flag | | |
| --fail-self-update | | Testing flag | | |
| --FD- | | | | |
| --force-auto-patch | | | | |
| --force-device-scale-factor | Float | Overrides OS DPI scaling | `--force-device-scale-factor=1` | |
| --force-move-install | | | | |
| --fuzz-testing | | | | |
| --games | | | | |
| --get-on-subscribe | | | | |
| --gtest_break_on_failure | | | | |
| --headless | | Runs the client without a visible window | `--headless` | |
| --heap-inspector | | | | |
| --ignore-plugin-dependencies | | | | |
| --insecure | | Disables SSL certificate verification | `--insecure` | |
| --install-directory | String | | | |
| --installer-dir | String | | | |
| --installer-start-agent | | | | |
| --install-flow | | | | |
| --install-path | String | | | |
| --install-tracker-dir | String | | | |
| --landing-token | String | | | |
| --launch-background-mode | | | | |
| --launcher- | | | | |
| --launcher-disable-self-update | | | | |
| --launcher-sync-with-subscriber | | | | |
| --launcher-system-yaml-override | String | | | |
| --launcher-test-port | Integer | | | |
| --launch-patchline | String | | | |
| --launch-product | String | | | |
| --league-client-id | String | | | |
| --locale | String | Sets the UI language | `--locale=en_US` | |
| --log | | | | |
| --log-dir | String | | `--log-dir=""` | |
| --login | | | | |
| --log-root | String | | | |
| --log-rotation-count | Integer | | | |
| --log-rotation-size | Integer | | | |
| --log-subdir | String | | `--log-subdir=""` | |
| --mem-mon-enabled | | Enables memory monitoring | | |
| --mem-mon-interval | Integer | Memory monitor poll interval | | |
| --mem-mon-mem-delta | Integer | Memory delta threshold | | |
| --mem-mon-pf-delta | Integer | Page fault delta threshold | | |
| --mem-mon-reg-delta | Integer | Registry delta threshold | | |
| --patchline | String | | | |
| --persistence-path | String | | | |
| --player-session-lifecycle | | | | |
| --plugins-path | String | | | |
| --post-restart | | | | |
| --priority-launch-path | String | | | |
| --priority-launch-pid | Integer | | | |
| --product | String | | | |
| --product-install-patchline | String | | | |
| --product-install-path | String | | | |
| --product-install-root | String | | | |
| --product-shortcut-path | String | | | |
| --quick-launch | | | | |
| --quiet | | Suppresses output | `--quiet` | |
| --region | String | Sets the server region | `--region=NA` | |
| --remoting-auth-token | String | | | |
| --remoting-tracing | | | | |
| --repair-permissions | | | | |
| --reparo-- | | | | |
| --replay-command-stream | | | | |
| --respawn-command | String | | | |
| --respawn-display-name | String | | | |
| --restart-timestamp | Integer | | | |
| --riotclient-app-port | Integer | | `--riotclient-app-port=12345` | |
| --riotclient-auth-token | String | Authentication token for RCS | `--riotclient-auth-token=ivA3Yi-u5aqUd_0q1ATCZM` | |
| --riotclient-dev-mode | | Enables developer mode | | |
| --riotclient-dir | String | | | |
| --riotclient-port-range | String | | | |
| --riotclient-release-id | String | | | |
| --rms-url | String | | | |
| --rso-auth | | | | |
| --rso_original_platform_id | String | | | |
| --rso_platform_id | String | | | |
| --scd-url | String | | | |
| --scheduler-stack-size | Integer | | | |
| --scheduler-tracing | | | | |
| --scheduler-tracing-quieter | | | | |
| --seconds | Integer | | | |
| --servers | String | | | |
| --session-id | String | | | |
| --shard | String | | | |
| --show-dev-tools | | Opens DevTools window | `--show-dev-tools` | |
| --show-dev-tools-all | | Opens DevTools for all windows | | |
| --show-swagger | | Exposes the Swagger UI | `--show-swagger` | |
| --skip-to-install | | | | |
| --stay-signed-in | | | | |
| --sync-with-subscriber | | | | |
| --system-yaml-override | String | Overrides system YAML config | `--system-yaml-override=""` | |
| --tencent | | Tencent-specific flow | | |
| --test-automation-pid | Integer | | | |
| --test-session-id | String | | | |
| --thirdparty | | | | |
| --tsi | | | | |
| --type | String | | | |
| --uninstall | | Triggers uninstall flow | `--uninstall` | |
| --uninstall-patchline | String | | | |
| --uninstall-pid | Integer | | | |
| --uninstall-product | String | | | |
| --update-root | String | | | |
| --upgrade-flow | | | | |
| --upgrade-install-path | String | | | |
| --upgrade-patchline | String | | | |
| --upgrade-product | String | | | |
| --url | String | | | |
| --use-http | | Forces HTTP instead of HTTPS | `--use-http` | |
| --user-data-root | String | | | |
| --ux-helper-name | String | | `--ux-helper-name=""` | |
| --ux-name | String | | `--ux-name=""` | |
| --ux-path | String | | | |
| --vmodule | String | | | |
| --working-directory | String | | | |

---

## Riot Client.exe — Chromium / Node.js / V8 flags

These flags are passed to the Electron/CEF host process and are processed by Chromium, Node.js, or V8.

> **Note:** Some entries in this section appear to be parser artifacts or embedded data fragments from the binary (e.g. `--MultipartBoundary-`, `--StartFragment`, `--SS--`, `--towardsRecords...`). They are listed here verbatim for completeness.

| Argument | What it does | Notes |
|:---|:---|:---|
| --abcdefghijklmnopqrstuvwxyz------abcdefghijklmnopqrstuvwxyz-------------------------------------------------------------------------------------------------------------------------------------____ | | Artifact |
| --abort-on-uncaught-exception | Aborts process on uncaught JS exception | Node.js |
| --addons | | Node.js |
| --always-turbofan | Forces TurboFan JIT for all code | V8 |
| --American | | Artifact |
| --annotation | | |
| --apk-embedded-library | | Chromium |
| --aq_mode | | Video encoder (libaom/libvpx) |
| --arm_arch | | Compiler/build |
| --attachment | | |
| --BEGH | | Artifact |
| --BEGIN | | Artifact |
| --build-snapshot | | Node.js |
| --bytecode-old-age | | V8 |
| --call-graph-size | | |
| --check | Syntax-check scripts without executing | Node.js |
| --checkForUpdate | | Electron |
| --compact-code-space-with-stack | | V8 |
| --compact-maps | | V8 |
| --compact-with-stack | | V8 |
| --compiler | | |
| --completion-bash | | Node.js CLI |
| --concurrent-sparkplug | | V8 |
| --concurrent-sparkplug-high-priority-threads | | V8 |
| --concurrent-sparkplug-max-threads | | V8 |
| --conditions | | Node.js |
| --Controlclassescoveredoutlineattacksdevices | | Artifact |
| --correctness-fuzzer-suppressions | | V8 fuzzer |
| --cpu-prof | Writes a CPU profile on exit | Node.js |
| --cpu-prof-dir | Output directory for CPU profiles | Node.js |
| --cpu-prof-interval | Sampling interval in µs | Node.js |
| --cpu-prof-name | Output filename for CPU profile | Node.js |
| --cq-level | | Video encoder |
| --crash-on-aborted-evacuation | | V8 |
| --csa-trap-on-node | | V8 CSA |
| --D--- | | Artifact |
| --D------ | | Artifact |
| --Daniel | | Artifact |
| --database | | |
| --debug | | Node.js (legacy) |
| --debug-arraybuffer-allocations | | V8 |
| --debug-brk | Break before user code starts | Node.js |
| --debug-port | | Node.js |
| --deltaq-mode | | Video encoder |
| --demangle | | Profiler |
| --deprecation | | Node.js |
| --diagnostic-dir | Directory for diagnostic output | Node.js |
| --disable-gl-error-limit | Removes the GL error log cap | Chromium |
| --disable-gpu | Disables GPU hardware acceleration | Chromium |
| --disable-ipc-flooding-protection | Removes IPC message rate limits | Chromium |
| --disable-proto | | Node.js |
| --disallow-code-generation-from-strings | | V8 |
| --distortion | | Video encoder |
| --dns-result-order | | Node.js |
| --D--R | | Artifact |
| --D--R--R | | Artifact |
| --DS--- | | Artifact |
| --DS-RR | | Artifact |
| --dynamicFrame | | |
| --en_US | | Locale artifact |
| --enable_chroma_deltaq | | Video encoder |
| --enable-automation | Marks the browser as controlled by automation | Chromium |
| --enable-experimental-regexp-engine-on-excessive-backtracks | | V8 |
| --enable-features | Comma-separated list of Chromium features to enable | Chromium |
| --enable-fips | Enables FIPS-compliant crypto | Node.js |
| --enable-sharedarraybuffer-per-context | | V8 |
| --enable-source-maps | Enables source map support | Node.js |
| --enable-tpl-model | | Video encoder |
| --EndFragment-- | | Artifact (clipboard HTML) |
| --ENDH | | Artifact |
| --end-usage | | Video encoder (rate control) |
| --es-module-specifier-resolution | | Node.js |
| --eval | Evaluates a script argument | Node.js |
| --experimental-abortcontroller | | Node.js |
| --experimental-fetch | | Node.js |
| --experimental-flush-embedded-blob-icache | | V8 |
| --experimental-global-customevent | | Node.js |
| --experimental-global-webcrypto | | Node.js |
| --experimental-import-meta-resolve | | Node.js |
| --experimental-json-modules | | Node.js |
| --experimental-loader | | Node.js |
| --experimental-modules | | Node.js |
| --experimental-network-imports | | Node.js |
| --experimental-policy | | Node.js |
| --experimental-relaxed-simd | | V8 / WASM |
| --experimental-repl-await | | Node.js |
| --experimental-report | | Node.js |
| --experimental-specifier-resolution | | Node.js |
| --experimental-top-level-await | | Node.js |
| --experimental-vm-modules | | Node.js |
| --experimental-wasi-unstable-preview1 | | Node.js |
| --experimental-wasm-eh | | V8 / WASM |
| --experimental-wasm-gc | | V8 / WASM |
| --experimental-wasm-memory64 | | V8 / WASM |
| --experimental-wasm-modules | | V8 / WASM |
| --experimental-wasm-ref-cast-nop | | V8 / WASM |
| --experimental-wasm-return_call | | V8 / WASM |
| --experimental-wasm-simd | | V8 / WASM |
| --experimental-wasm-stack-switching | | V8 / WASM |
| --experimental-wasm-stringref | | V8 / WASM |
| --experimental-wasm-threads | | V8 / WASM |
| --experimental-wasm-typed_funcref | | V8 / WASM |
| --experimental-wasm-typed-funcref | | V8 / WASM |
| --experimental-wasm-type-reflection | | V8 / WASM |
| --experimental-worker | | Node.js |
| --expose_wasm | | V8 |
| --expose-gc | Exposes `gc()` global in JS | V8 |
| --expose-internals | | Node.js |
| --external | | |
| --extIdx | | |
| --female | | Artifact |
| --filter-runtime-timer | | V8 |
| --finalize-streaming-on-background | | V8 |
| --finishCount | | |
| --fixed-qp-offsets | | Video encoder |
| --flag | | |
| --flush-baseline-code | | V8 |
| --flush-bytecode | | V8 |
| --force_marking_deque_overflows | | V8 |
| --force-async-hooks-checks | | Node.js |
| --force-context-aware | | Electron |
| --force-fips | Forces FIPS-compliant crypto | Node.js |
| --force-node-api-uncaught-exceptions-policy | | Node.js |
| --frame | | |
| --frameHash | | |
| --framePath | | |
| --framePosition | | |
| --frozen-intrinsics | | Node.js |
| --future | | V8 |
| --GBK1-0 | | Artifact (charset name) |
| --gc-experiment-reduce-concurrent-marking-tasks | | V8 |
| --gc-memory-reducer-start-delay-ms | | V8 |
| --Glagolitic | | Artifact |
| --global-search-paths | | |
| --growJSONdutyNamesaleyou | | Artifact |
| --harmony | Enables all ES-next harmony features | V8 |
| --harmony-array-grouping | | V8 |
| --harmony-atomics | | V8 |
| --harmony-import-assertions | | V8 |
| --harmony-sharedarraybuffer | | V8 |
| --harmony-struct | | V8 |
| --heap-prof | Writes a heap profile on exit | Node.js |
| --heap-prof-dir | Output directory for heap profiles | Node.js |
| --heap-prof-interval | Sampling interval | Node.js |
| --heap-prof-name | Output filename for heap profile | Node.js |
| --heapsnapshot-near-heap-limit | | Node.js |
| --heap-snapshot-near-heap-limit | | Node.js |
| --heapsnapshot-signal | | Node.js |
| --help | Prints help text | Node.js |
| --http-parser | | Node.js |
| --huge-max-old-generation-size | | V8 |
| --icu-data-dir | | Node.js |
| --ignore-unknown | | |
| --immediateInfo | | |
| --info-log-- | | |
| --initial-client-data | | Electron |
| --input-type | | Node.js |
| --insecure-http-parser | | Node.js |
| --inspect | Activates inspector on host:port | Node.js |
| --inspect-brk | Break before user code + inspector | Node.js |
| --inspect-brk-node | | Node.js |
| --inspect-port | Inspector port | Node.js |
| --inspect-publish-uid | | Node.js |
| --interactive | Forces REPL even with non-tty stdin | Node.js |
| --interpreted-frames-native-stack | | V8 |
| --isolated-prerender-tunnel-proxy | | Chromium |
| --jitless | Disables JIT compilation | V8 |
| --lazy-feedback-allocation | | V8 |
| --left | | |
| --liftoff | | V8 / WASM |
| --liftoff-only | | V8 / WASM |
| --linux | | Platform artifact |
| --loader | | Node.js |
| --log-code | | V8 |
| --logfile | | |
| --lossless | | |
| --maglev | | V8 |
| --maxdepth | | |
| --max-http-header-size | Max HTTP header size in bytes | Node.js |
| --max-old-space-size | Max heap size in MB | V8 |
| --maxvars | | |
| --metrics-dir | | Node.js |
| --monitor-self | | |
| --monitor-self-annotation | | |
| --monitor-self-argument | | |
| --MultipartBoundary- | | Artifact (multipart HTTP) |
| --MultipartBoundary-- | | Artifact (multipart HTTP) |
| --napi-modules | | Node.js |
| --no-addons | | Node.js |
| --no-compact-code-space-with-stack | | V8 |
| --no-compact-maps | | V8 |
| --no-compact-with-stack | | V8 |
| --no-concurrent-sparkplug | | V8 |
| --no-concurrent-sparkplug-high-priority-threads | | V8 |
| --no-crash-on-aborted-evacuation | | V8 |
| --node-memory-debug | | Node.js |
| --no-deprecation | Suppresses deprecation warnings | Node.js |
| --node-snapshot | | Node.js |
| --no-enable-experimental-regexp-engine-on-excessive-backtracks | | V8 |
| --no-experimental-flush-embedded-blob-icache | | V8 |
| --no-experimental-repl-await | | Node.js |
| --no-experimental-wasm-simd | | V8 |
| --no-expose-wasm | | V8 |
| --no-finalize-streaming-on-background | | V8 |
| --no-flag | | |
| --no-flush-baseline-code | | V8 |
| --no-flush-bytecode | | V8 |
| --no-freeze-flags-after-init | | V8 |
| --no-future | | V8 |
| --no-gc-experiment-reduce-concurrent-marking-tasks | | V8 |
| --no-harmony-array-grouping | | V8 |
| --no-harmony-impcaught-exception--abort-on-uncaucaught_exception--abort_on_uncauX | | Artifact |
| --no-harmony-sharedarraybuffer | | V8 |
| --noharmony-shipping | | V8 |
| --no-identify-client-via-url | | |
| --no-inline-new | | V8 |
| --no-lazy-feedback-allocation | | V8 |
| --no-liftoff | | V8 |
| --no-maglev | | V8 |
| --no-opt | Disables JIT optimization | V8 |
| --no-periodic-tasks | | V8 |
| --no-rate-limit | | |
| --no-reclaim-unmodified-wrappers | | Node.js |
| --no-sandbox | **Disables the Chromium sandbox** | Chromium — security risk |
| --no-short-builtin-calls | | V8 |
| --no-slow-histograms | | V8 |
| --no-sparkplug | | V8 |
| --no-sparkplug-needs-short-builtins | | V8 |
| --no-stress-per-context-marking-worklist | | V8 |
| --no-turbo-fast-api-calls | | V8 |
| --no-upload-gzip | | |
| --no-use-map-space | | V8 |
| --no-warnings | Suppresses process warnings | Node.js |
| --no-wasm-dynamic-tiering | | V8 |
| --no-wasm-lazy-compilation | | V8 |
| --no-wasm-tier-up | | V8 |
| --no-wasm-write-protect-code-memory | | V8 |
| --no-write-protect-code-memory | | V8 |
| --objdump | | Profiler |
| --only-summary | | |
| --openssl-config | | Node.js |
| --openssl-shared-config | | Node.js |
| --optimize_for_size | | V8 |
| --optimize-for-size | Optimizes V8 for memory over speed | V8 |
| --original-shader-- | | Artifact |
| --other | | |
| --pairs | | |
| --pairwise-timed-range | | Video encoder |
| --pending | | |
| --pending-deprecation | | Node.js |
| --perf-basic-prof | | Node.js (Linux) |
| --perf-basic-prof-only-functions | | Node.js (Linux) |
| --perf-prof | | Node.js (Linux) |
| --perf-prof-unwinding-info | | Node.js (Linux) |
| --pipe-name | | |
| --policy-integrity | | Node.js |
| --port | | |
| --POST | | Artifact |
| --preprocess | | |
| --preserve-symlinks | | Node.js |
| --preserve-symlinks-main | | Node.js |
| --print | | Node.js |
| --processStartAndWait | | |
| --prof | V8 profiler output | V8 |
| --profile-electron-init | | Electron |
| --prof-process | Processes V8 profiler output | V8 |
| --prop | | |
| --range | | |
| --reclaim-unmodified-wrappers | | Node.js |
| --redirect-warnings | | Node.js |
| --report-compact | | Node.js |
| --report-dir | | Node.js |
| --report-directory | | Node.js |
| --report-filename | | Node.js |
| --report-on-fatalerror | | Node.js |
| --report-on-signal | | Node.js |
| --report-signal | | Node.js |
| --report-uncaught-exception | | Node.js |
| --require | Pre-loads a CommonJS module | Node.js |
| --script-delay | | |
| --script-delay-fraction | | |
| --script-delay-once | | |
| --secure-heap | | Node.js |
| --secure-heap-min | | Node.js |
| --security-revert | | Node.js |
| --security-reverts | | Node.js |
| --separate-builtins | | V8 |
| --separate-bytecodes | | V8 |
| --separate-ic | | V8 |
| --separate-sparkplug-handlers | | V8 |
| --separate-stubs | | V8 |
| --serialize-vm-symbols | | V8 |
| --shared-string-table | | V8 |
| --short-builtin-calls | | V8 |
| --slow-histograms | | V8 |
| --source-map | | Node.js |
| --sparkplug | | V8 |
| --sparkplug-needs-short-builtins | | V8 |
| --SS-- | | Artifact |
| --SSRR | | Artifact |
| --SSS--- | | Artifact |
| --SSSRRR | | Artifact |
| --SSSS | | Artifact |
| --SSSSSS | | Artifact |
| --stack-trace-limit | Max stack frames in traces | V8 |
| --StartFragment | | Artifact (clipboard HTML) |
| --StartFragment-- | | Artifact (clipboard HTML) |
| --state | | |
| --stress_compaction | | V8 |
| --stress-marking | | V8 |
| --stress-per-context-marking-worklist | | V8 |
| --stress-scavenge | | V8 |
| --target | | |
| --templateStackDepth | | |
| --test | | Node.js |
| --test-only | | Node.js |
| --test-udp-no-try-send | | Node.js |
| --this | | |
| --throw-deprecation | Throws on deprecated API use | Node.js |
| --timed-range | | Video encoder |
| --title | Sets process title | Node.js |
| --tls-cipher-list | | Node.js |
| --tls-keylog | | Node.js |
| --tls-max-v1 | | Node.js |
| --tls-min-v1 | | Node.js |
| --toFinish | | |
| --towardsRecordsPrivateForeignPremierchoicesVirtualreturnsCommentPoweredinline | | Artifact |
| --trace_all_uses | | V8 |
| --trace_representation | | V8 |
| --trace_turbo | | V8 TurboFan |
| --trace_turbo_alloc | | V8 TurboFan |
| --trace_turbo_ceq | | V8 TurboFan |
| --trace_turbo_graph | | V8 TurboFan |
| --trace_turbo_jt | | V8 TurboFan |
| --trace_turbo_loop | | V8 TurboFan |
| --trace_turbo_reduction | | V8 TurboFan |
| --trace_turbo_scheduled | | V8 TurboFan |
| --trace_turbo_stack_accesses | | V8 TurboFan |
| --trace_turbo_trimming | | V8 TurboFan |
| --trace-atomics-wait | | Node.js |
| --trace-deprecation | | Node.js |
| --trace-event-categories | | Node.js |
| --trace-event-file-pattern | | Node.js |
| --trace-events-enabled | | Node.js |
| --trace-exit | | Node.js |
| --trace-osr | | V8 |
| --trace-sigint | | Node.js |
| --trace-sync-io | | Node.js |
| --trace-tls | | Node.js |
| --trace-uncaught | | Node.js |
| --trace-warnings | | Node.js |
| --track-heap-objects | | V8 |
| --track-retaining-path | | V8 |
| --translated-shader-- | | Artifact |
| --turbofan | | V8 |
| --turbo-fast-api-calls | | V8 |
| --type | | |
| --unhandled-rejections | | Node.js |
| --update | | |
| --use_fixed_qp_offsets | | Video encoder |
| --use_strict | | V8 |
| --use-bundled-ca | | Node.js |
| --use-largepages | | Node.js |
| --use-map-space | | V8 |
| --use-openssl-ca | | Node.js |
| --user-data-dir | Chromium user data directory | Chromium |
| --use-strict | | Node.js |
| --v8-options | Prints all V8 options | V8 |
| --v8-pool-size | Sets the V8 thread pool size | V8 |
| --valid | | |
| --verbose | | |
| --verify-base-objects | | V8 |
| --version | Prints version string | Node.js |
| --warnings | | Node.js |
| --wasm-dynamic-tiering | Enables WASM dynamic tiering | V8 |
| --wasm-lazy-compilation | Enables lazy WASM compilation | V8 |
| --wasm-staging | Enables staged / experimental WASM features | V8 |
| --wasm-tier-up | Enables WASM tier-up to TurboFan | V8 |
| --wasm-write-protect-code-memory | Write-protects WASM code memory | V8 |
| --WebKitFormBoundary | | Artifact (multipart form) |
| --windows | | Platform artifact |
| --write-protect-code-memory | | V8 |
| --Y-Yh | | Artifact |
| --zero-fill-buffers | Zero-fills Buffer allocations | Node.js |

---

## CEF / Chromium highlights

The following Chromium flags are of particular interest when working with the Riot Client's embedded browser.

| Argument | What it does |
|:---|:---|
| --disable-gl-error-limit | Removes the GL error log cap |
| --disable-gpu | Disables GPU hardware acceleration (software rendering) |
| --disable-ipc-flooding-protection | Removes IPC message rate limits |
| --disable-proto | |
| --enable-automation | Marks the browser as controlled by automation |
| --enable-features | Comma-separated list of Chromium feature flags to enable |
| --no-sandbox | **Disables the Chromium sandbox — security risk** |
| --user-data-dir | Path to the Chromium profile directory |
| --v8-options | Passes additional options to V8 |
| --v8-pool-size | Sets the V8 thread pool size |
| --wasm-dynamic-tiering | Enables WASM dynamic tiering |
| --wasm-lazy-compilation | Enables lazy WASM compilation |
| --wasm-staging | Enables staged / experimental WASM features |
| --wasm-tier-up | Enables WASM tier-up to TurboFan |
| --wasm-write-protect-code-memory | Write-protects WASM code memory |

