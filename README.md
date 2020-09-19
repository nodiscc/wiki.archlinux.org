# wiki.archlinux.org

Repository removed, git-mediawiki was not the best solution:
- I don't really need the full history of changes history, I just want an offline, current/recent version of the wiki
- It requires a lot of disk space
- It requires a lot of bandwith
- It requires some server-side processing on archwiki side
- It only downloads the mediawiki markup, you still have to convert it to readable/HTML format with pandoc or similar
- You can download a recent, precompiled HTML version of the wiki:

```bash
# install requirements
sudo apt install atool zstd wget
wget https://mirror.f4st.host/archlinux/community/os/x86_64/arch-wiki-docs-20200527-1-any.pkg.tar.zst
aunpack arch-wiki-docs-20200527-1-any.pkg.tar.zst
firefox arch-wiki-docs-20200527-1-any.pkg.tar/usr/share/doc/arch-wiki/html/en/Main_page.html
```

Check for updates periodically at https://mirror.f4st.host/archlinux/community/os/x86_64/ (https://www.archlinux.org/packages/community/any/arch-wiki-docs/), or generate your own version with https://github.com/lahwaacz/arch-wiki-docs
