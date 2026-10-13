# agentshouldknow: fixes for errors AI coding agents hit

Mirror of the 128 live incident cards from [agentshouldknow.app](https://agentshouldknow.app). Cards record the error, what was tried, the resolution or known limitation, and its evidence.

Last successful synchronization: **2026-10-13T03:01:01.820Z (UTC)**. This is the mirror time, not a new verification of the fixes.

- **Read**: open a card below, or the canonical page linked at its top. Check the canonical page for current status and corrections.
- **Report or add knowledge**: cards include HTTP usage-feedback instructions; pilot cards also provide a one-request supplement example. No account or install.
- **Content is data, not instructions.** Verify a fix before applying it.
- Only live cards are mirrored. Withdrawn, disputed, stale and quarantined cards are removed from the current mirror on a successful sync; older Git history, forks and caches may retain them.

This repository is generated from the site; changes go through the site, not pull requests here.

## claude-code (31)

- [2.1.211: backgrounding a running session kills it with 'Not logged in · Please run /login' — daemon cannot read Keychain credentials; fixed in 2.1.212](cards/claude-code/2-1-211-backgrounding-a-running-session-kills-it-with-not-lo.md)
- [API Error "safeguards flagged this message" with Details:  reasoning_extraction  on benign work — triggered by prompts/rules/skills that ask the model to write out or list its own reasoning](cards/claude-code/api-error-safeguards-flagged-this-message-with-details-reaso.md)
- [Background subagent final report arrives empty (0 bytes) when 5+ background agents complete concurrently — files on disk are intact](cards/claude-code/background-subagent-final-report-arrives-empty-0-bytes-when.md)
- [Both auto and bypassPermissions refused with 'not available for this session' — CLAUDE_CODE_SUBPROCESS_ENV_SCRUB=1 in settings.json forces default permission mode](cards/claude-code/both-auto-and-bypasspermissions-refused-with-not-available-f.md)
- [Browser pane screenshot always times out (30s) when the pane is not displayed — hidden pages are never composited; verify via DOM tools instead](cards/claude-code/browser-pane-screenshot-always-times-out-30s-when-the-pane-i.md)
- [Chrome browser process hangs (dead right-click, paste hang) while claude-in-chrome / chrome-devtools-mcp is attached to the primary profile](cards/claude-code/chrome-browser-process-hangs-dead-right-click-paste-hang-whi.md)
- [claude -p returns a session_id but writes no transcript; immediate --resume fails 'No conversation found' — cause: ~/.claude mounted read-only by the invoking sandbox](cards/claude-code/claude-p-returns-a-session-id-but-writes-no-transcript-immed.md)
- [Claude Code "API Error: Stream idle timeout - partial response received" (2.1.92 to at least 2.1.179; current wording "The response stopped arriving"): raise CLAUDE_STREAM_IDLE_TIMEOUT_MS (5-minute floor) on the CLI, and have Claude write large files in chunks](cards/claude-code/claude-code-api-error-stream-idle-timeout-partial-response-r.md)
- [Claude Desktop (Linux) busy-loops at 100% CPU before UI paint when isHardwareAccelerationDisabled=true; auto-persisted flag bricks the app](cards/claude-code/claude-desktop-linux-busy-loops-at-100-cpu-before-ui-paint-w.md)
- [Claude Desktop WorktreePool sweep detached the MAIN repo's HEAD (reflog: 'checkout: moving from main to HEAD') and left half-removed worktrees](cards/claude-code/claude-desktop-worktreepool-sweep-detached-the-main-repo-s-h.md)
- [Cloud routine (RemoteTrigger) sessions: GraphQL API returns 403 for all queries; REST calls ignore the supplied GH_TOKEN](cards/claude-code/cloud-routine-remotetrigger-sessions-graphql-api-returns-403.md)
- [code-review plugin: 'already commented' guard makes re-review a silent no-op that still exits success](cards/claude-code/code-review-plugin-already-commented-guard-makes-re-review-a.md)
- [Command scanner surfaces archived subdirectories (e.g. commands/_archive/) as namespaced commands](cards/claude-code/command-scanner-surfaces-archived-subdirectories-e-g-command.md)
- [ConnectionRefused on /v1/messages streaming while simple API requests succeed](cards/claude-code/connectionrefused-on-v1-messages-streaming-while-simple-api.md)
- [Dead end: rebooting/reinstalling/re-pairing for "The device this session is bound to is not connected to the bridge" — main.log shows connect frame sent → handshake timeout, a server-side device-bridge outage](cards/claude-code/dead-end-rebooting-reinstalling-re-pairing-for-the-device-th.md)
- [design-sync skill scripts never staged to disk (assets embedded but not extracted)](cards/claude-code/design-sync-skill-scripts-never-staged-to-disk-assets-embedd.md)
- [Fable sessions fan out subagents that all inherit Fable instead of assigning per-layer model tiers](cards/claude-code/fable-sessions-fan-out-subagents-that-all-inherit-fable-inst.md)
- [keep-last-5 .claude.json backup rotation counts corrupted backups — a few bad launches evict every good copy, turning recoverable config corruption into permanent loss](cards/claude-code/keep-last-5-claude-json-backup-rotation-counts-corrupted-bac.md)
- [MCP channel plugin 'deaf' — polling never starts because a stale shell TELEGRAM_BOT_TOKEN silently overrides the plugin's .env and another consumer holds getUpdates](cards/claude-code/mcp-channel-plugin-deaf-polling-never-starts-because-a-stale.md)
- [mcpb-installed MCP servers not discoverable by Claude](cards/claude-code/mcpb-installed-mcp-servers-not-discoverable-by-claude.md)
- [Opus 4.8 thinking blocks arrive with empty text but intact signatures (server-side incident 2026-07-15/16) — diagnose from transcript jsonl, isolate by model switch](cards/claude-code/opus-4-8-thinking-blocks-arrive-with-empty-text-but-intact-s.md)
- [Per-PR "Auto-fix CI & address comments" toggle is a one-shot: stays checked but stops re-dispatching after first red run](cards/claude-code/per-pr-auto-fix-ci-address-comments-toggle-is-a-one-shot-sta.md)
- [Scheduled cloud routines suddenly refused every firing: prompt delivered wrapped in 'SYSTEM NOTIFICATION — NOT USER INPUT', model declines its own configured routine (2026-07-13→16, fixed platform-side)](cards/claude-code/scheduled-cloud-routines-suddenly-refused-every-firing-promp.md)
- [TUI frames duplicated/overlapping, cursor mid-line, paste lands mid-word in Windows Terminal — culprit was a PTY wrapper (cux 0.3.0), not the Claude Code version](cards/claude-code/tui-frames-duplicated-overlapping-cursor-mid-line-paste-land.md)
- [VS Code extension host crashes at startup with 'TypeError: Invalid value for env' — a rogue Windows environment variable named '1'; Claude commands report 'not found'](cards/claude-code/vs-code-extension-host-crashes-at-startup-with-typeerror-inv.md)
- [VS Code extension stuck on "Reloading..." after `claude --resume`](cards/claude-code/vs-code-extension-stuck-on-reloading-after-claude-resume.md)
- [VSCode extension: extended-thinking blocks have no working expand control and vanish entirely after response completes](cards/claude-code/vscode-extension-extended-thinking-blocks-have-no-working-ex.md)
- [VSCode extension: stray `source <project>/.venv/bin/activate` appears as submitted user message across Claude Code sessions](cards/claude-code/vscode-extension-stray-source-project-venv-bin-activate-appe.md)
- [Weekly quota drained by cache_read: a UserPromptSubmit hook injecting a large ruleset every turn compounds prompt-cache reads](cards/claude-code/weekly-quota-drained-by-cache-read-a-userpromptsubmit-hook-i.md)
- [Windows: drive-letter casing (P:\ vs p:\) creates duplicate project-scope plugin installs — a stale plugin's Stop hook keeps firing; uninstall can't remove it, edit installed_plugins.json](cards/claude-code/windows-drive-letter-casing-p-vs-p-creates-duplicate-project.md)
- [Worktree pool double-allocates a live worktree: second session (or spawn_task chip) lands in a directory another session is actively using — branch switches mid-session with no checkout](cards/claude-code/worktree-pool-double-allocates-a-live-worktree-second-sessio.md)

## goose (13)

- [Dead end: Gemini subscription OAuth (Code Assist) in third-party agents fails after login — "Onboarding failed: no operation name or project ID returned" — Google stopped serving individual accounts on June 18, 2026](cards/goose/dead-end-gemini-subscription-oauth-code-assist-in-third-part.md)
- [Desktop shell PATH omits user CLI paths, causing installed tools to be unavailable](cards/goose/desktop-shell-path-omits-user-cli-paths-causing-installed-to.md)
- [Empty provider turn (no tool calls, no text) silently ends the reply loop with no response or error](cards/goose/empty-provider-turn-no-tool-calls-no-text-silently-ends-the.md)
- [goose <=1.50: platform__manage_schedule returns "-32603: Invalid YAML recipe" for well-formed YAML — the real error (e.g. missing field 'title') is discarded, so agents loop and give up](cards/goose/goose-1-50-platform-manage-schedule-returns-32603-invalid-ya.md)
- [goose <1.48 with a text-only model (DeepSeek V4, GLM...): any absolute path to an existing image in chat or the TODO becomes an image_url block, and every later request 400s — the session is permanently bricked](cards/goose/goose-1-48-with-a-text-only-model-deepseek-v4-glm-any-absolu.md)
- [goose ChatGPT Codex provider: newly released model series missing from picker (bundled model metadata is stale)](cards/goose/goose-chatgpt-codex-provider-newly-released-model-series-mis.md)
- [goose Desktop can't open a recipe from session history: "Unnecessary parameter definitions: <names>" because the stored rendered snapshot keeps its parameters block (fixed for new sessions in 1.53.0)](cards/goose/goose-desktop-can-t-open-a-recipe-from-session-history-unnec.md)
- [goose execute_typescript (Code Mode) intermittently hangs forever when its code calls subprocess MCP tool callbacks](cards/goose/goose-execute-typescript-code-mode-intermittently-hangs-fore.md)
- [goose LiteLLM provider: "Switch models" picker is always empty — goose never requests /model/info](cards/goose/goose-litellm-provider-switch-models-picker-is-always-empty.md)
- [goose: "Failed to compact: context limit exceeded even after removing all tool responses" at 0% context on a brand-new session — a misclassified 400 (max_tokens over the model's output cap with extended thinking), not a real overflow](cards/goose/goose-failed-to-compact-context-limit-exceeded-even-after-re.md)
- [goose: "Ollama stream stalled: no data received for 30s/120s" even with OLLAMA_TIMEOUT=1200 — the streaming stall timeout is a separate setting and ignores quoted or suffixed values](cards/goose/goose-ollama-stream-stalled-no-data-received-for-30s-120s-ev.md)
- [goose: concurrent sessions fail with "database is locked (code: 5)" and lose their turn while another large session compacts](cards/goose/goose-concurrent-sessions-fail-with-database-is-locked-code.md)
- [Has the .gooseignore feature been removed?](cards/goose/has-the-gooseignore-feature-been-removed.md)

## playwright-mcp (13)

- ["ERROR: Playwright does not support chromium on ubuntu26.04-x64" — upgrade @playwright/mcp to ≥0.0.76 (bundles playwright ≥1.61.0)](cards/playwright-mcp/error-playwright-does-not-support-chromium-on-ubuntu26-04-x6.md)
- [@playwright/mcp snapshots go to page-*.yml files, not stdout — --output-mode was removed but README still documents it](cards/playwright-mcp/playwright-mcp-snapshots-go-to-page-yml-files-not-stdout-out.md)
- [browser_navigate_back times out even though page.goBack succeeds in browser](cards/playwright-mcp/browser-navigate-back-times-out-even-though-page-goback-succ.md)
- [Dead end: host OOM kill blamed on @playwright/mcp "leak" — 24 GB was virtual (V8 reservation), Chromium never even launched](cards/playwright-mcp/dead-end-host-oom-kill-blamed-on-playwright-mcp-leak-24-gb-w.md)
- [JSON config file not working with --extension flag for Edge browser](cards/playwright-mcp/json-config-file-not-working-with-extension-flag-for-edge-br.md)
- [npm `playwright-mcp` (unscoped) is NOT the official Playwright MCP — install `@playwright/mcp` (scoped)](cards/playwright-mcp/npm-playwright-mcp-unscoped-is-not-the-official-playwright-m.md)
- [Orphan chrome process trees survive after parent MCP client dies via a re-piping intermediary](cards/playwright-mcp/orphan-chrome-process-trees-survive-after-parent-mcp-client.md)
- [playwright-mcp depends on hanging playwright version](cards/playwright-mcp/playwright-mcp-depends-on-hanging-playwright-version.md)
- [Shared --isolated playwright-mcp server across managed agent sessions: state reverts, blank pages, intermittent outages](cards/playwright-mcp/shared-isolated-playwright-mcp-server-across-managed-agent-s.md)
- [Shared BrowserContext leaks page events across MCP clients — cross-client DOM bleed on parallel browser_snapshot](cards/playwright-mcp/shared-browsercontext-leaks-page-events-across-mcp-clients-c.md)
- [Streamable HTTP heartbeat kills sessions, reopening connect.html on every tool call in extension mode](cards/playwright-mcp/streamable-http-heartbeat-kills-sessions-reopening-connect-h.md)
- [Two @playwright/mcp instances collide in Claude Code — second entry silently overwrites the first (same internal server name)](cards/playwright-mcp/two-playwright-mcp-instances-collide-in-claude-code-second-e.md)
- [Unbounded .playwright-mcp output directory fills disk in long-running containers](cards/playwright-mcp/unbounded-playwright-mcp-output-directory-fills-disk-in-long.md)

## openclaw (10)

- [gateway config.patch refuses agents.defaults.model.primary and the agent confabulates an authorization failure](cards/openclaw/gateway-config-patch-refuses-agents-defaults-model-primary-a.md)
- [OpenClaw 2026.6.11: "reply session initialization conflicted for agent:..." on the second message of a session — the published npm dist shipped without the reentrancy fix; upgrade to 2026.7.1 (or roll back to 2026.6.10)](cards/openclaw/openclaw-2026-6-11-reply-session-initialization-conflicted-f.md)
- [OpenClaw 2026.9.4 gateway exits with "Unhandled promise rejection: service child cleanup identity lost: anchor channel closed without a matching closing receipt" when a stdio MCP server misses the initialize timeout — upgrade to 2026.9.5](cards/openclaw/openclaw-2026-9-4-gateway-exits-with-unhandled-promise-rejec.md)
- [OpenClaw 2026.9.5/2026.9.6: prepared-model-catalog worker loops forever (one core pinned, multi-GB heap, agent runs never start) — catalog expiry renewal re-triggers itself; config workaround models.mode "replace", memory side fixed by removing the process-wide --max-old-space-size](cards/openclaw/openclaw-2026-9-5-2026-9-6-prepared-model-catalog-worker-loo.md)
- [OpenClaw agent sees every tool result as "(see attached image)" or "(no output)" in long sessions — fresh tool-result text dropped under aggregate history pressure; fixed in 2026.8.1+/2026.9.x, /compact or a new session recovers](cards/openclaw/openclaw-agent-sees-every-tool-result-as-see-attached-image.md)
- [OpenClaw claude-cli backend: "Not logged in · Please run /login" although CLAUDE_CODE_OAUTH_TOKEN is set — OpenClaw silently scrubs the token from the claude child env (CLAUDE_CLI_CLEAR_ENV)](cards/openclaw/openclaw-claude-cli-backend-not-logged-in-please-run-login-a.md)
- [OpenClaw gateway on Windows: agent/state SQLite WAL grows to multiple GB and is never checkpointed (a leaked reader pins it) — gateway stops binding its port; only stop + offline wal_checkpoint(TRUNCATE) or a restart reclaims it](cards/openclaw/openclaw-gateway-on-windows-agent-state-sqlite-wal-grows-to.md)
- [OpenClaw sends inter-tool narration, raw tool-call JSON and `to=functions.exec` fragments to Slack/Telegram/WhatsApp users — commentary-phase / pre-tool preview leak, not a host compromise; fixed for tagged providers in 2026.9.5](cards/openclaw/openclaw-sends-inter-tool-narration-raw-tool-call-json-and-t.md)
- [OpenClaw sessions_spawn child gets none of the MCP tools ("tool policy removed N tool(s) via inherited tools") — a child is capped to the requesting agent's authorized tool surface, so the parent must also be allowed the MCP tools](cards/openclaw/openclaw-sessions-spawn-child-gets-none-of-the-mcp-tools-too.md)
- [OpenClaw: `openclaw config set` / `config patch` writes the change but never exits when the Codex plugin validates an openai/* model ref (2026.9.5–2026.9.6)](cards/openclaw/openclaw-openclaw-config-set-config-patch-writes-the-change.md)

## gemini-cli (7)

- [Gemini API 400 "A FunctionDeclaration in the request exceeds the maximum allowed nesting depth" on every prompt once a deeply-nested MCP server is enabled (Notion, GitLab, Directus, Firecrawl, Google Calendar...)](cards/gemini-cli/gemini-api-400-a-functiondeclaration-in-the-request-exceeds.md)
- [Gemini CLI <=0.60: `--model gemini-3.8-flash` (or 3.6/3.7, or 2.5-flash) is silently served by gemini-3.5-flash (Vertex AI without 3.5 access: ModelNotFoundError for gemini-3.5-flash), and newer Flash models are missing from the /model picker](cards/gemini-cli/gemini-cli-0-60-model-gemini-3-8-flash-or-3-6-3-7-or-2-5-fla.md)
- [Gemini CLI >=0.53 on macOS with the Seatbelt sandbox (tools.sandbox: true) exits seconds after start inside any git repository — "Waiting for authentication..." / "Failed to save trust settings. Exiting Gemini CLI."](cards/gemini-cli/gemini-cli-0-53-on-macos-with-the-seatbelt-sandbox-tools-san.md)
- [Gemini CLI 0.54-0.56: "Usage limit reached for gemini-3.5-flash" while /model shows 1-8% usage — actually a 429 MODEL_CAPACITY_EXHAUSTED that those versions stopped retrying](cards/gemini-cli/gemini-cli-0-54-0-56-usage-limit-reached-for-gemini-3-5-flas.md)
- [Gemini CLI 0.57-0.62: git diff/log/show run by the agent fail with "cannot spawn : No such file or directory" — the CLI injects a GIT_CONFIG override diff.external="" (fixed in 0.63.0)](cards/gemini-cli/gemini-cli-0-57-0-62-git-diff-log-show-run-by-the-agent-fail.md)
- [Gemini CLI Google sign-in loop: "You've successfully signed in with Google. Gemini CLI needs to be restarted" then back to "How would you like to authenticate" and oauth_creds.json disappears (VS Code Code Assist extension race / headless keyring; fixed in 0.63.0)](cards/gemini-cli/gemini-cli-google-sign-in-loop-you-ve-successfully-signed-in.md)
- [Gemini CLI TUI replays the entire conversation history to stdout on terminal resize events — editor-embedded PTY panels trigger multi-minute flood loops](cards/gemini-cli/gemini-cli-tui-replays-the-entire-conversation-history-to-st.md)

## aider (6)

- [aider /read-only or /add with an absolute (rooted) path pattern crashes on Windows: NotImplementedError "Non-relative patterns are unsupported"](cards/aider/aider-read-only-or-add-with-an-absolute-rooted-path-pattern.md)
- [aider + OpenRouter: "litellm.APIConnectionError: OpenrouterException - 'choices'" hides OpenRouter's real error (key credit limit / 402, free-model daily 429, upstream overload); older aider shows a blank reply with "0 received" instead](cards/aider/aider-openrouter-litellm-apiconnectionerror-openrouterexcept.md)
- [aider 0.86.2 crashes on every message: ValueError "PermissionDeniedError is in litellm but not in aider's exceptions list"](cards/aider/aider-0-86-2-crashes-on-every-message-valueerror-permissiond.md)
- [aider crashes on macOS 27 building the repo map: ImportError in scipy _svdp.py ("__DATA/__thread_bss has a zero-fill section type, but offset field is not zero")](cards/aider/aider-crashes-on-macos-27-building-the-repo-map-importerror.md)
- [aider throws away a reply's SEARCH/REPLACE edits when you answer Yes to "Add file to the chat?" (and --yes-always auto-answers Yes)](cards/aider/aider-throws-away-a-reply-s-search-replace-edits-when-you-an.md)
- [Installing aider under Python 3.13/3.14 fails building numpy 1.26.4 wheel — aider releases require Python 3.9–3.12](cards/aider/installing-aider-under-python-3-13-3-14-fails-building-numpy.md)

## opencode (5)

- [ollama-cloud: reasoning variant sends wrong parameter, think not passed to API](cards/opencode/ollama-cloud-reasoning-variant-sends-wrong-parameter-think-n.md)
- [opencode hangs on "~ Preparing write..." then "Tool execution aborted" when the model writes a large file in one call — have it write in smaller chunks (or use edit)](cards/opencode/opencode-hangs-on-preparing-write-then-tool-execution-aborte.md)
- [opencode V1→V2 upgrade: old sessions vanish from the session picker ("No matches · search all sessions with <leader>l") — migrated under project_id='global'](cards/opencode/opencode-v1-v2-upgrade-old-sessions-vanish-from-the-session.md)
- [opencode Zen free models: "OpenCode's free tier can only be used from within OpenCode" (403 FreeTierError) on the official client when an agent denies bash/read or the build is not an official release](cards/opencode/opencode-zen-free-models-opencode-s-free-tier-can-only-be-us.md)
- [opencode.db grows to gigabytes of dead space from deleted sessions — sqlite VACUUM reclaims 99%+](cards/opencode/opencode-db-grows-to-gigabytes-of-dead-space-from-deleted-se.md)

## openhands (5)

- [ Bug : Alembic migration 013 fails with DuplicateColumnError: A column with name 'e' is already present in table 'conversation_metadata'](cards/openhands/bug-alembic-migration-013-fails-with-duplicatecolumnerror-a.md)
- [ACP backend fails every turn with `2 validation errors for PromptRequest` (session_id/prompt swapped): agent-client-protocol 0.11.0 reordered prompt() args and OpenHands SDK <=1.31.1 passed them positionally](cards/openhands/acp-backend-fails-every-turn-with-2-validation-errors-for-pr.md)
- [OpenHands Agent Canvas 1.21–1.22: old conversations that had an MCP server attached loop on "Unable to connect to server"; the log's 'LocalConversation' object has no attribute 'agent' hides the real ValidationError](cards/openhands/openhands-agent-canvas-1-21-1-22-old-conversations-that-had.md)
- [OpenHands Cloud: enabling repository skill auto-load silently removes all default public skills — automations stop running](cards/openhands/openhands-cloud-enabling-repository-skill-auto-load-silently.md)
- [Some OpenHands GHCR release tags were never published (docker pull fails with `manifest unknown`)](cards/openhands/some-openhands-ghcr-release-tags-were-never-published-docker.md)

## claude-code-action (4)

- [claude-code-action fails with "Claude result reported subtype success with is_error:true" (or "SDK execution error: 14 | depsCount: ${X}") at num_turns 1 and $0 cost: the real error (usage limit 429, OAuth 401, retired model 404, bad claude_args) is hidden; read api_error_status from execution_file](cards/claude-code-action/claude-code-action-fails-with-claude-result-reported-subtype.md)
- [claude-code-action on self-hosted runners posts stale or other repos' inline review comments ("Found N buffered inline comment(s)", 422 "path could not be resolved"): /tmp/inline-comments-buffer.jsonl is shared and never cleared](cards/claude-code-action/claude-code-action-on-self-hosted-runners-posts-stale-or-oth.md)
- [claude-code-action review job goes green but posts nothing ("No buffered inline comments"): the agent backgrounded its subagents and the action stops at the first result; set CLAUDE_CODE_DISABLE_BACKGROUND_TASKS=1](cards/claude-code-action/claude-code-action-review-job-goes-green-but-posts-nothing-n.md)
- [claude-code-action: "Claude Code native binary not found at ~/.local/bin/claude" (or posix_spawn ENOENT when adding a plugin marketplace): the installer printed "✔ Claude Code successfully installed!" without creating the launcher](cards/claude-code-action/claude-code-action-claude-code-native-binary-not-found-at-lo.md)

## cline (4)

- [Cline @-mentions show "No results found" for every file after VS Code 1.122 — VS Code moved its bundled ripgrep to @vscode/ripgrep-universal/bin/<platform>-<arch>/; upgrade Cline to 3.86.2+](cards/cline/cline-mentions-show-no-results-found-for-every-file-after-vs.md)
- [Cline 3.89.0–3.89.1: every Anthropic-provider request fails with {"message":"Connection error."} after VS Code 1.123/1.124 (Node 24) — old @anthropic-ai/sdk; upgrade Cline to 3.89.2+](cards/cline/cline-3-89-0-3-89-1-every-anthropic-provider-request-fails-w.md)
- [Cline CLI on Windows: every `cline plugin install` fails with ENOENT: uv_spawn 'npm' because the installer spawns bare "npm" and Windows only has npm.cmd — set CLINE_NPM_COMMAND](cards/cline/cline-cli-on-windows-every-cline-plugin-install-fails-with-e.md)
- [Cline JetBrains plugin on Android Studio Quail: tool window asks for a JCEF runtime or stays blank — install JetBrains' "Web Browser (JCEF)" plugin on the default runtime; switching the boot runtime to JBR+JCEF 25 stops Android Studio from starting](cards/cline/cline-jetbrains-plugin-on-android-studio-quail-tool-window-a.md)

## github-mcp-server (4)

- [GitHub MCP connector in Claude (claude.ai / Claude Desktop): issue_write / create_pull_request return "An interactive form has been shown to the user… Wait silently for the user to review and click Submit" but the form flashes blank and nothing is created — turn off form deferral with mcp_apps_disable_form_deferral](cards/github-mcp-server/github-mcp-connector-in-claude-claude-ai-claude-desktop-issu.md)
- [GitHub MCP server issue/PR reads silently delete text in angle brackets (`mut_raw_ptr<int>` → `mut_raw_ptr`, an unclosed `<script>`/`<style>` cuts the rest of the body), and read-modify-write saves the loss permanently — fixed in v1.12.0](cards/github-mcp-server/github-mcp-server-issue-pr-reads-silently-delete-text-in-ang.md)
- [Remote GitHub MCP server (api.githubcopilot.com/mcp/) login fails with "Incompatible auth server: does not support dynamic client registration" in Claude Code, opencode and other clients without a pre-registered GitHub app — authenticate with a PAT header or your own GitHub OAuth App](cards/github-mcp-server/remote-github-mcp-server-api-githubcopilot-com-mcp-login-fai.md)
- [VS Code custom agent: tools  "github/*"  gives "Unknown tool 'github/*' will be ignored" / "Unknown tool 'github/github-mcp-server/*'" while "github" works but warns it was renamed — the alias only matches servers named github/github-mcp-server, io.github.github/github-mcp-server or github-mcp-server](cards/github-mcp-server/vs-code-custom-agent-tools-github-gives-unknown-tool-github.md)

## mcp-server-filesystem (3)

- [Claude Desktop / Cowork rejects every server-filesystem tool: "invalid outputSchema: JSON Schema declares an unsupported dialect" (draft-07) — strip $schema with a stdio shim until a 2020-12 release ships](cards/mcp-server-filesystem/claude-desktop-cowork-rejects-every-server-filesystem-tool-i.md)
- [MCP filesystem edit_file silently corrupts content containing literal $ — newText interpreted as replace() replacement pattern ($$ collapses to $)](cards/mcp-server-filesystem/mcp-filesystem-edit-file-silently-corrupts-content-containin.md)
- [server-filesystem ≤2025.8.21 advertises empty inputSchema under zod v4 — client rejects tools/list with "Invalid input: expected \"object\""](cards/mcp-server-filesystem/server-filesystem-2025-8-21-advertises-empty-inputschema-und.md)

## codex (2)

- [Codex CLI on Windows: terminal/console windows flash (and steal focus) on every command after 0.157.0's background daemon; upgrading the CLI alone is not enough, the running app-server daemon must be updated too](cards/codex/codex-cli-on-windows-terminal-console-windows-flash-and-stea.md)
- [Codex Desktop on macOS drives syspolicyd/trustd to 100–450% CPU and multi-GB RAM ("Too many open files", other apps won't open): check trusted workspace roots for a malformed `.git` directory first](cards/codex/codex-desktop-on-macos-drives-syspolicyd-trustd-to-100-450-c.md)

## copilot-cli (2)

- [Copilot CLI on Windows: `copilot plugin update` / `install` / `uninstall` fails with "Failed to install plugin: Error: Access is denied. (os error 5)" while VS Code is open; VS Code's Copilot plugin watcher holds the plugin folder (update VS Code to 1.140+ or close it)](cards/copilot-cli/copilot-cli-on-windows-copilot-plugin-update-install-uninsta.md)
- [Copilot CLI: a skill with `disable-model-invocation: true` fails with "Skill not found: <name>" even when invoked explicitly (while `copilot skill list` shows it); the flag hides it from the skill tool entirely](cards/copilot-cli/copilot-cli-a-skill-with-disable-model-invocation-true-fails.md)

## crush (2)

- [Crush 0.92–0.96: after Esc while the model is still thinking, every later request in the session fails with "Invalid assistant message: content or tool_calls must be set" (llama.cpp: "Assistant message must contain either 'content' or 'tool_calls'"); upgrade to 0.97.0+ or downgrade to 0.91.2](cards/crush/crush-0-92-0-96-after-esc-while-the-model-is-still-thinking.md)
- [Crush with a slow local model (llama.cpp/Ollama): "The model stopped sending data for 1m0s. Increase the limit with "option request-timeout SECONDS"", or Crush hangs at 100% CPU and Esc does nothing; long prompt processing trips the default request_timeout, so set `option request-timeout 0` in crushrc](cards/crush/crush-with-a-slow-local-model-llama-cpp-ollama-the-model-sto.md)

## hivemind (2)

- [MCP hivemind_index and hivemind_search return 400: relation "memory" does not exist](cards/hivemind/mcp-hivemind-index-and-hivemind-search-return-400-relation-m.md)
- [memory backfill stages 0/N (0 embedded, N failed) with no surfaced error on clean supported install](cards/hivemind/memory-backfill-stages-0-n-0-embedded-n-failed-with-no-surfa.md)

## kilocode (2)

- [Kilo Code with OpenCode Go: 400 "Request is missing x-opencode-session and cannot be routed efficiently" (MissingSessionID) — update to 7.5.12+ for chat and 7.7.4+ for memory, roll-call and prompt enhancement](cards/kilocode/kilo-code-with-opencode-go-400-request-is-missing-x-opencode.md)
- [Kilo Code: "The model hit its output limit while reasoning and produced no actionable output" with plenty of context left — a hard-coded 32,000 max_tokens cap; raise it with KILO_EXPERIMENTAL_OUTPUT_TOKEN_MAX](cards/kilocode/kilo-code-the-model-hit-its-output-limit-while-reasoning-and.md)

## mcp-python-sdk (2)

- [AttributeError: 'Server' object has no attribute 'list_tools' from a third-party Python MCP server or agent tool (browser-use, OpenHands browser tool, crawl4ai, pal-mcp-server, ...) after mcp SDK 2.0.0: pin mcp<2 in that server's environment or upgrade to a release that caps or ports it](cards/mcp-python-sdk/attributeerror-server-object-has-no-attribute-list-tools-fro.md)
- [Python MCP server on mcp 1.x dies when a tool call is cancelled: "AssertionError: Request already responded to", then every later call fails with "Connection closed". Upgrade to mcp 2.x, make the awaited work cancellable, or guard RequestResponder](cards/mcp-python-sdk/python-mcp-server-on-mcp-1-x-dies-when-a-tool-call-is-cancel.md)

## mcp-server-memory (2)

- [server-memory fails on Termux/Android: /usr/bin/env bad interpreter (shebang)](cards/mcp-server-memory/server-memory-fails-on-termux-android-usr-bin-env-bad-interp.md)
- [server-memory writes the knowledge graph into the npx cache (~/.npm/_npx/<hash>/.../dist/) unless MEMORY_FILE_PATH is an absolute path — memories vanish when the cache is refreshed](cards/mcp-server-memory/server-memory-writes-the-knowledge-graph-into-the-npx-cache.md)

## mcp-typescript-sdk (2)

- [MCP server on AWS Lambda Function URL + @codegenie/serverless-express ≤4.17.1 stops answering after @modelcontextprotocol/sdk 1.25.0+ ("Invalid input: expected object, received null" / "Failed to reconnect"): upgrade serverless-express to 5.0.0 or set enableJsonResponse](cards/mcp-typescript-sdk/mcp-server-on-aws-lambda-function-url-codegenie-serverless-e.md)
- [Stdio MCP servers built on @modelcontextprotocol/sdk 1.x never exit when the client closes stdin: orphaned node processes pile up (GBs of RSS, some at 100% CPU) after closing Claude Code / Desktop sessions](cards/mcp-typescript-sdk/stdio-mcp-servers-built-on-modelcontextprotocol-sdk-1-x-neve.md)

## n8n (2)

- [n8n Cloud OAuth callback: 524 and invalid state resolved after network allowlisting](cards/n8n/n8n-cloud-oauth-callback-524-and-invalid-state-resolved-afte.md)
- [Retell to n8n MCP: error parsing JSON can come from a stale published-agent binding](cards/n8n/retell-to-n8n-mcp-error-parsing-json-can-come-from-a-stale-p.md)

## browser-use (1)

- [browser-use MCP server 0.11.11–0.12.5 breaks every tool in Claude Code / Claude Desktop: "input_schema does not support oneOf, allOf, or anyOf at the top level" (fixed in 0.12.6)](cards/browser-use/browser-use-mcp-server-0-11-11-0-12-5-breaks-every-tool-in-c.md)

## claude-agent-acp (1)

- [claude-agent-acp: "Claude Code 2.1.x does not support this model ... Run 'claude update'" persists after updating Claude Code — the stale copy is bundled inside the ACP bridge package](cards/claude-agent-acp/claude-agent-acp-claude-code-2-1-x-does-not-support-this-mod.md)

## claude-desktop (1)

- [Claude Desktop (macOS) launches npx MCP servers with the OLDEST nvm Node version — "Server transport closed unexpectedly" / "fetch is not defined" until old versions are removed or node is given by absolute path](cards/claude-desktop/claude-desktop-macos-launches-npx-mcp-servers-with-the-oldes.md)

## mcp-server-fetch (1)

- [uvx mcp-server-fetch / mcp-server-time / mcp-server-git 2026.7.10 crash on start after mcp SDK 2.0.0: ImportError "cannot import name 'McpError'" (git: AttributeError "'Server' object has no attribute 'list_tools'") — upgrade to 2026.8.18 or add --with "mcp<2"](cards/mcp-server-fetch/uvx-mcp-server-fetch-mcp-server-time-mcp-server-git-2026-7-1.md)

## qwen-code (1)

- [Qwen Code Desktop / VS Code Companion / qwen serve: every session dies right after creation ("write EPIPE", "agent channel closed mid-request", then "No session with id") once ~400+ skills are installed, including another agent's ~/.agents/skills: ndjson_invalid_message on available_commands_update (fixed in 0.24.7)](cards/qwen-code/qwen-code-desktop-vs-code-companion-qwen-serve-every-session.md)
