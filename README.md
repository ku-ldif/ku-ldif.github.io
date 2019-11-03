# ku-ldif.github.io

Kyoto University LDIF Daisuki Club (ja: 京都大学 LDIF 同好会) <https://ku-ldif.github.io/>

This project uses [ldap2html](https://github.com/nonylene/ldap2html) for converting LDIF to html.

## Guide

### Add documents

LDIF files (`XXX-*.html.ldif`) under the `src` directory will be passed to `ldapadd` in alphabetical order.

### Modify documents

**DON'T MODIFY LDIF, DO ADD NEW LDIF.**

If you want to modify existing docuemnts, use `ldapmodify`.

LDIF files (`XXX-*.html.ldif`) under the `src/modify` directory will be passed to `ldapmodify` after all `ldapadd`s.

## License

See [LICENSE](./LICENSE).
