# Start with a set you love

[← Home](../README.md) · [简体中文](GETTING-STARTED.zh-CN.md)

DJ Set Tracker is a desktop browser extension for YouTube and Bilibili. Use the current Chrome or Edge browser.

## Install from a store

Choose [Chrome Web Store](https://chromewebstore.google.com/detail/set-tracker/jdpgcgcbigjpgfheaimikbkmgdpkaaod) or [Microsoft Edge Add-ons](https://microsoftedge.microsoft.com/addons/detail/set-tracker/dicipdfdgkemhcflmngpgojnhoialnoj), install the extension, then refresh any video tabs already open. Store releases update through the browser after approval.

## Install the latest ZIP

1. Open [Latest release](https://github.com/BlackiePiggy/DJ-Set-Tracker/releases/latest) and download **DJ-Set-Tracker-Chrome-Edge.zip** under **Assets**. Do not download “Source code (zip)”.
2. Extract the ZIP to a permanent folder, such as `DJ-Set-Tracker`. Keep the extracted files there after installation.
3. Open `chrome://extensions` in Chrome or `edge://extensions` in Edge. Enable **Developer mode**.
4. Choose **Load unpacked** and select the extracted folder containing `manifest.json`. This package has its manifest at the root of the ZIP.
5. Open or refresh a YouTube / Bilibili video. Click the floating **SET TRACKER** button on the right.

The same ZIP works in both browsers. A store installation and an unpacked installation are separate extensions and may have separate local data; avoid enabling both at once.

## Follow your first tracklist

1. Open a DJ set video and expand the SET TRACKER panel.
2. Pick an available tracklist from the tracklist selector. If none is available, open **Import / Sources**.
3. You can bring in a 1001Tracklists URL, scan loaded description/comment text, or import a text/CSV tracklist. Review the preview before applying it.
4. Play the video. The current track follows playback; click another cue to jump to it.

For description/comment scanning, expand the description and load the comments you want to scan first. If a source site requests verification, complete it normally in the source page, then retry the import.

## Dial in the timing

Different uploads can have different intros or edits. Use the quick timing controls to adjust the tracklist offset; **Reset** returns it to zero. A positive offset moves track cues later in the video. Check more than one cue: a single offset cannot correct cuts made halfway through a recording.

## Save a find or contribute

Sign in inside the extension to use account features such as favorites. Save individual tracks or whole tracklists, then revisit them from **My library**. Music-platform actions open a supplied link or search when a direct link is unavailable; an exact mix or version may not exist on every service.

Use the editor to add tracks and mark cue times against playback. Review imported or matched titles, artists and times before publishing. Reading a song link shows a preview; choose **Use cover and details** to adopt it. Importing or saving an editing draft does not by itself publish a community tracklist.

## Update a ZIP installation

1. Read the [new release notes](https://github.com/BlackiePiggy/DJ-Set-Tracker/releases/latest) and download the ZIP.
2. Extract the new version separately. Close editing views and finish saving any work first.
3. Replace the extension files in the **same folder used for the previous unpacked installation** with the new package contents. Keep that folder path unchanged.
4. Click **Reload** on the existing extension card in `chrome://extensions` or `edge://extensions`.
5. Refresh video tabs and confirm the new version on the extension card.

Do not remove the extension merely to update it: removal can erase local drafts and settings. Browser profiles and different extension IDs have separate storage. GitHub ZIP installations need these manual updates; they do not receive automatic GitHub updates.

To hear about releases, select **Watch → Custom → Releases** on this repository.

## Quick answers

**No floating button?** Confirm the extension is enabled, refresh the video, and use a desktop `www.youtube.com` or `www.bilibili.com` video page. Mobile apps are not supported. Your browser may need permission to let the extension run on the video site.

**No tracklist for this set?** Coverage depends on available sources and community contributions. Import a matching source or create a list. DJ Set Tracker does not listen to the audio to identify every track automatically.

**A cue is off?** Confirm the source is for the same recording and edit. Adjust the offset for a fixed delay, or correct individual cue times when needed.

**An ID or a music link is missing?** Unknown tracks and unreleased edits are common in DJ sets. Keep the uncertainty instead of substituting a different recording. Search results are suggestions, not proof of a match.

**The store has a different version?** Store review and GitHub publishing follow independent schedules. Use the actual version displayed by your browser; a GitHub release does not mean the same version is already approved in either store.

**Can I verify the download?** Every release includes `SHA256SUMS.txt`. Compare the ZIP hash with `shasum -a 256 DJ-Set-Tracker-Chrome-Edge.zip` on macOS/Linux, or `Get-FileHash .\DJ-Set-Tracker-Chrome-Edge.zip -Algorithm SHA256` in Windows PowerShell.

**Need help?** [Open an issue](https://github.com/BlackiePiggy/DJ-Set-Tracker/issues/new/choose) with the browser, extension version, public video URL and steps to reproduce. Do not include passwords, tokens or private account information. [Website support](https://djsettracker.live/support) · [Privacy policy](https://djsettracker.live/privacy).
