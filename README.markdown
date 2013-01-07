# classpath.vim

This plugin sets the `'path'` for JVM languages to match the class path of
your current Java project.  This lets commands like `:find` and `gf` work as
designed.  I originally wrote it for Clojure, but I see no reason why it
wouldn't be handy for other languages as well.

Currently, [Maven][] and [Leiningen][] are supported, with a fallback to
`$CLASSPATH` if neither applies.  [Open an issue][GitHub issues] if you have
ideas for supporting another project management system.

Included is a `:Java` command, which executes `java` (or `$JAVA_CMD`) with the
current buffer's `'path'` as the class path.

[Maven]: http://maven.apache.org/
[Leiningen]: https://github.com/technomancy/leiningen
[GitHub issues]: https://github.com/tpope/vim-classpath/issues

## Installation

If you don't have a preferred installation method, I recommend
installing [pathogen.vim](https://github.com/tpope/vim-pathogen), and
then simply copy and paste:

    cd ~/.vim/bundle
    git clone git://github.com/tpope/vim-classpath.git

Once help tags have been generated, you can view the manual with
`:help classpath`.

## Contributing

See the contribution guidelines for
[pathogen.vim](https://github.com/tpope/vim-pathogen#readme).

## Self-Promotion

Like classpath.vim?  Follow the repository on
[GitHub](https://github.com/tpope/vim-classpath).  And if
you're feeling especially charitable, follow [tpope](http://tpo.pe/) on
[Twitter](http://twitter.com/tpope) and
[GitHub](https://github.com/tpope).

## License

Copyright © Tim Pope.  Distributed under the same terms as Vim itself.
See `:help license`.
