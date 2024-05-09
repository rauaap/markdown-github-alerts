# markdown-github-alerts

Alerts extension for [Python-Markdown](https://github.com/Python-Markdown/markdown). Replaces Github style alert blocks with the appropriate HTML. Styling is not included, but can be acquired from [here](https://github.com/sindresorhus/github-markdown-css) for example.

## Installation

```bash
pip install markdown-github-alerts
```

## Example

This would be replaced:

````
> [!NOTE]
> This is a note.
````

With this:

```html
<div class="markdown-alert markdown-alert-note">
    <p class="markdown-alert-title">
        <svg class="octicon octicon-info mr-2" height="16" viewBox="0 0 16 16" width="16">
            <path d="M0 8a8 8 0 1 1 16 0A8 8 0 0 1 0 8Zm8-6.5a6.5 6.5 0 1 0 0 13 6.5 6.5 0 0 0 0-13ZM6.5 7.75A.75.75 0 0 1 7.25 7h1a.75.75 0 0 1 .75.75v2.75h.25a.75.75 0 0 1 0 1.5h-2a.75.75 0 0 1 0-1.5h.25v-2h-.25a.75.75 0 0 1-.75-.75ZM8 6a1 1 0 1 1 0-2 1 1 0 0 1 0 2Z"></path>
        </svg>Note
    </p>
    <p>This is a note.</p>
</div>
```

Which looks like this with Github css:

> [!NOTE]
> This is a note.

