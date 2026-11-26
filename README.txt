VOLTAGE LOGGER - build your APK with GitHub (no installs needed)

1. Sign in at github.com (free account), tap + > New repository. Name it e.g. voltage-logger. Keep it Private. Create.
2. Click "uploading an existing file". Drag in: package.json, capacitor.config.json, and the www folder (index.html inside it). Commit.
3. Click Add file > Create new file. In the name box type exactly:
      .github/workflows/build.yml
   Open build-workflow.yml from this zip in a text editor, copy everything, paste it in. Commit.
4. Open the Actions tab. The "Build APK" run starts by itself (about 5-8 minutes). Wait for the green tick.
5. Click the finished run, scroll to Artifacts, download voltage-logger-apk (a zip containing app-debug.apk).
6. Unzip, send the APK to your phone, tap it and allow "install unknown apps" when asked.
7. Open Voltage Logger, tap Start listening, allow the microphone.

If the run fails (red cross): open the run, click the failed step, copy the last ~30 lines of the log and send them to Claude.
