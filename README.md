# ku-ldif.github.io

![Status badge](https://github.com/ku-ldif/ku-ldif.github.io/workflows/Build/badge.svg)

Kyoto University LDIF Daisuki Club (ja: 京都大学 LDIF 同好会) <https://ku-ldif.github.io/>

This project uses [ldap2html](https://github.com/nonylene/ldap2html) for converting LDIF to HTML.

## Guide

HTML documents are auto-generated and pushed by [CI (GitHub Actions)](https://github.com/ku-ldif/ku-ldif.github.io/actions).

Source LDIF files and generated HTML documents are under the `gh-pages` branch.

### Add documents

LDIF files (`*.html.ldif`) under the `src` directory will be passed to `ldapadd`.

### Modify documents

**DON'T MODIFY LDIF, DO ADD NEW LDIF.**

If you want to modify existing docuemnts, use `ldapmodify`.

LDIF files (`XXX-*.html.ldif`) under the `src/modify` directory will be passed to `ldapmodify` in alphabetical order, after all `ldapadd`s.

## License

See [LICENSE](./LICENSE).
