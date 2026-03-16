 (cd "$(git rev-parse --show-toplevel)" && git apply --3way <<'EOF' 
diff --git a/README.md b/README.md
new file mode 100644
index 0000000000000000000000000000000000000000..ecb515ccdaeb6da90823470e7c82a9edd6c4278d
--- /dev/null
+++ b/README.md
@@ -0,0 +1,68 @@
+# Underworld Datapack (Minecraft 1.21.11)
+
+This datapack adds a custom Nether biome named **Underworld** that appears deep below the Nether around **Y -100**.
+
+## What it adds
+
+- **Biome ID:** `underworld:underworld`
+- **World preset ID:** `underworld:underworld`
+- A dark teal sky tint in biome effects.
+- Flat-ish mycelium plains generated via large mycelium disks.
+- Random soul sand patches.
+- Random green crystal-like blocks (`verdant_froglight`) as crystal growths.
+
+## Download file (easy to find)
+
+If you are browsing this repo, download this file directly:
+
+- `Underworld-Datapack-1.21.11.zip`  ← top-level zip at repo root
+
+A copy is also kept here:
+
+- `dist/Underworld-Datapack-1.21.11.zip`
+
+## Installation (singleplayer)
+
+1. Open Minecraft and create/select a world.
+2. Open the world folder (`Edit` -> `Open World Folder`).
+3. Open the `datapacks` folder.
+4. Copy `Underworld-Datapack-1.21.11.zip` into `datapacks`.
+5. Start the world and run `/reload`.
+
+## Installation (new world with custom Nether preset)
+
+To get the custom Nether generation setup from world creation:
+
+1. Place this datapack in the world's `datapacks` folder before first load.
+2. Create a **new world** and choose world preset `underworld:underworld`.
+3. Enter the Nether and go to around **Y -100** to find Underworld regions.
+
+## Notes
+
+- This pack modifies Nether biome selection through a custom world preset, so it works best on newly created worlds.
+- Existing Nether chunks will not retroactively regenerate.
+
+## If you want a real GitHub download button
+
+GitHub only shows an obvious download flow if the file is in a repo (or a Release).
+
+### Quickest way (just upload the zip)
+
+1. Create a new repo on GitHub.
+2. Click **Add file** -> **Upload files**.
+3. Upload `Underworld-Datapack-1.21.11.zip`.
+4. Open that file on GitHub and click **Download raw file**.
+
+### Better way (GitHub Release with Assets)
+
+1. In your repo, go to **Releases** -> **Draft a new release**.
+2. Tag it like `v1.0.0`.
+3. In **Attach binaries**, upload `Underworld-Datapack-1.21.11.zip`.
+4. Publish release.
+5. Share the release URL — users get a clear download button under **Assets**.
+
+### If users only have the repo URL
+
+They can still click **Code** -> **Download ZIP**, but that downloads the whole repo,
+not just the datapack file.
+
 
EOF
)
