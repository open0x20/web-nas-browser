# web-nas-browser
A file browser that looks like an old MS-DOS command line. Written in PHP.

![Screenshot of a directory with mouse hovering over archlinux iso](/docs/example-view.png)

### Setup
1. Copy the file into the root directory of your share.
2. Replace `$lowest_allowed_directory` with the root directory of your share.

### Special features
* Files with the extension `.link` will be treated as links. The target location has to be the content of the link file.
  ```
  Filename: take-me-to-example.org.link
  Contents: https://example.org/
  ```
* `.DS_STORE` and `index.php` files will not appear in a directory listing.
* Your IP will be displayed as part of the header.