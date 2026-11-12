# Polaris Dialogue Style — Active

Status: Mandatory interactive-story presentation rule
Applies to: Every spoken response from Polaris in current and future Gamer sessions

## Visual treatment

- A soft, light-blue, rounded bubble/box like a chat message.
- Background color: `#EAF6FF`.
- Text color: `#183A57`.
- Rounded corners and comfortable interior padding.
- Render her speech as ordinary readable text without surrounding quotation marks.
- **Never use a code block or a gray code panel for Polaris dialogue.**
- Keep Polaris visually distinct from narration, other characters, and mechanical status panels.

## Rendering fallback

Where custom color and rounded containers are supported, use the styled container. Where they are not, write Polaris's words as their own plain paragraph without quotes. Do not convert her words into fenced code to compensate for missing styling.

## Scope

This governs Polaris's conversation, including questions, explanations, jokes, and answers. System notifications, menus, and stat displays may remain separately formatted as required by the story's interface. Preserve `Prologue.md` as the original authored text; this rule governs continuation and display, not retroactive rewriting.

## Example

In a light-blue rounded bubble:

*Hello, D. Would you like me to display your current status?*

This example is italicized only to distinguish it in the Markdown reference file. Actual Polaris dialogue should use normal, non-italic text in the colored box.
