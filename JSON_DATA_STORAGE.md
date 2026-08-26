# JSON Form Data Storage

All submitted form data is stored as JSON.

- Static/local mode: data is saved in browser `localStorage` under `fureverFormData`.
- PHP server mode: each submission is also appended to `data/form-submissions.json` by `save-data.php`.
- Use **Download JSON Data** in the portal sidebar to export the browser-saved JSON.
- The veterinarian image itself is not embedded in JSON; its file name, MIME type, and size are saved.
