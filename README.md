# Alfred – iA Writer Inbox Doc

This Alfred workflow lets you quickly create a new iA Writer Markdown document in a configurable “inbox” folder and start typing immediately.

## Features

- Keyword: `doc`
- Creates a new `.md` file in a user-defined folder (your own “inbox” directory).
- Uses your typed text as:
  - The filename (`Your title.md`)
  - The first-level heading in the file (`# Your title`)
- Opens the new file directly in iA Writer.
- Optional Alfred notification confirming creation.

## Installation

1. Download the latest `.alfredworkflow` file from this repository.
2. Double-click the file to import it into Alfred.
3. Open **Alfred Preferences → Workflows** and select **iA Writer – Inbox Doc**.

## Configuration (choose your own inbox folder)

This workflow is configurable; you do **not** need to use any particular folder name.

1. In Alfred, with the workflow selected, click **Configure…** (or the workflow’s configuration button).
2. Under **Workflow Environment Variables**, find:
   - `inbox_folder`
3. Set `inbox_folder` to the full path of the folder where you want new notes saved, for example:

   - `/Users/yourname/Documents/Notes`
   - `/Users/yourname/Library/Mobile Documents/iCloud~com~iawriter~iA-Writer/Documents/Inbox`

4. Close the configuration window to save.

## Usage

- Bring up Alfred.
- Type:

  - `doc Your title` → creates `Your title.md` in your inbox folder.
  - `doc` (no title) → creates `Quick Note.md` (the default title).

- The workflow will:
  1. Create the Markdown file in `inbox_folder`.
  2. Insert `# Your title` (or `# Quick Note`) as the first line.
  3. Open the file in **iA Writer** and bring it to the front.
  4. Optionally show an Alfred notification that `"Your title.md" was created.

## Requirements

- macOS
- Alfred with Powerpack
- iA Writer for macOS installed

## Notes

- To change the keyword from `doc` to something else, double-click the **Keyword** object in the workflow and edit the keyword.
- The default title used when you type only `doc` can be changed in the **Args & Vars** object by editing the placeholder from `{query:Quick Note}` to your preferred text.
