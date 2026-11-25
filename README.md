# yoDEV Mail: Bulwark Webmail source code

yoDEV webmail (webmail.yodev.dev) runs [Bulwark Webmail](https://github.com/bulwarkmail/webmail), which is licensed
under the GNU Affero General Public License v3.0. As section 13 of that license requires, the complete source code
of the exact build we run is published here.

Each [release](https://github.com/yoDEV-dev/bulwark-source/releases) holds:

- `bulwark-yodev-<commit>-source.tar.gz`: the complete source of that build
- `SHA256SUMS`: the checksum of the source archive

## What we changed

Our build is upstream Bulwark with these changes, each described in `YODEV.md` in the archive:

- the icon an iPhone shows for webmail added to its home screen follows the webmail's branding settings, instead of
  always showing the Bulwark logo (from `f2a59cd`);
- a plugin with the new `calendar:invite` permission can send the invitations of an event it creates, so our AI
  plugin's "Make a meeting" can invite the people the member ticks (from `eaf9afb`).

| Release | Upstream base | Running on webmail.yodev.dev since |
|---|---|---|
| `v1.21.3-yodev-eaf9afb` | 1.21.3 | 2026-11-25 |
| `v1.21.3-yodev-f2a59cd` | 1.21.3 | 2026-11-25 to 2026-11-25 |

## License

Bulwark Webmail is © Bulwark Project Authors, licensed under AGPL-3.0 (`LICENSE`; `NOTICE` holds the attribution for
earlier MIT-licensed work). Our changes are released under the same license. The yoDEV name and {yo} logo are not
covered by it.
