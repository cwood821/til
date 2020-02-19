# Today I Learned

This repository tracks the snippets, notes, and ephemera that don't warrant a blog post but may prove useful later.
Inspired by [Josh Branchaud](https://github.com/jbranchaud/til) and [Chuck Grimmet](http://www.cagrimmett.com/til/).

107 notes and counting...

---

### Categories
- [Awk](#awk)
- [Bash](#bash)
- [CSS](#css)
- [Data Structures](#data-structures)
- [Docker](#docker)
- [Drupal](#drupal)
- [ElasticSearch](#elasticsearch)
- [Git](#git)
- [JavaScript](#javascript)
- [Jest](#jest)
- [Laravel](#laravel)
- [MongoDB](#mongodb)
- [MySQL](#mysql)
- [Networking](#networking)
- [Node](#node)
- [Numpy](#numpy)
- [PHP](#php)
- [PHPUnit](#phpunit)
- [Python](#python)
- [React](#react)
- [Rust](#rust)
- [SQLite](#sqlite)
- [SQL Server](#sql-server)
- [Theory](#theory)
- [Tmux](#tmux)
- [Unix](#unix)
- [Vagrant](#vagrant)
- [Video](#video)
- [Vim](#vim)


#### Awk
- [Get index of character in string](notes/awk/get-index-of-character-in-string.md)
- [Set separator between print statements](notes/awk/set-separator-between-print.md)

#### Bash
- [Get PID of shell running script](notes/bash/get-pid-of-shell-running-script.md)
- [Mark variables as readonly](notes/bash/mark-variables-as-readonly.md)
- [Use arrays in Bash](notes/bash/use-arrays.md)

#### CSS 
- [Target dark mode with media query](notes/css/target-dark-mode-with-media-query.md)
- [Typeset numbers for tables with font-feature-settings](notes/css/typset-font-numbers-for-tables.md)
- [Use `font-display: swap;` to render text in fallback font until @font-face font loads](notes/css/font-swap-in-css.md)

#### Data Structures 
- [Deque (double-ended queue)](notes/data-structures/deque.md)

#### Docker
- [Prune unused images and volumes](notes/docker/prune-unused-images.md)
- [Start Bash inside container](notes/docker/start-bash-inside-docker-container.md)

#### Drupal
- [Add an unlinked item to the breadcrumb in Drupal 8](notes/drupal/add-unlinked-item-to-drupal-breadcrumb.md)
- [Dump all Twig variable names in the current context](notes/drupal/dump-all-twig-variable-names.md)
- [Import updated configuration without uninstalling module](notes/drupal/import-updated-configuration.md)
- [List all registered plugin IDs for blocks with Drush](notes/drupal/list-registered-plugin-ids-for-blocks.md)
- [Get URL of current page in Drupal Twig](notes/drupal/get-url-of-current-page-drupal-twig.md)
- [Use optional configuration with modules](notes/drupal/use-optional-configuration-with-modules.md)

#### ElasticSearch
- [List indices on an ElasticSearch cluster](notes/elasticsearch/list-indices.md)

#### Git
- [Ammend previous commit message](notes/git/ammend-previous-commit-message.md)
- [Create patches](notes/git/create-patches-with-git.md)
- [Discard untracked changes](/notes/git/discard-untracked-changes.md)
- [Get path to root of repository](notes/git/get-path-to-repo-root.md)
- [Hide untracked files in git status](notes/git/hide-untracked-files-in-git-status.md)
- [List branches merged (or not) with current branch](notes/git/list-merged-git-branches.md)
- [Mark releases with tags](notes/git/mark-releases-with-tags.md)
- [Remove stale remote tracking branches](notes/git/remote-stale-remote-tracking-branches.md)
- [Revert file to some previous commit](notes/git/revert-file-to-previous-commit.md)
- [Search across historical commit diffs](notes/git/search-historical-commit-diffs.md)
- [See diff between current and last commit](notes/git/see-diff-between-current-and-last-commit.md)
- [Sign commits with GPG](notes/git/sign-git-commits-with-gpg.md)
- [Show only filenames in git log output](notes/git/show-only-filenames-in-git-log.md)
- [Stash and unstash changes](notes/git/stash-and-unstash-changes-in-git.md)

#### Jest
- [Define `window.location.href` for an individual test](notes/jest/define-window-location-for-individual-test.md)
- [Filter tests run by title](notes/jest/filter-test-run-by-title.md)

#### JavaScript
- [Convert an integer to hex, octal, or binary](notes/javascript/convert-integers-to-other-bases.md)
- [Make an enum-like structure with `Object.freeze`](notes/javascript/make-enum-like-structure.md)
- [Maps keep key insertion order and are iterable](notes/javascript/maps-keep-key-insertion-order.md)
- [Send message to parent window from iframe or popup](notes/javascript/send-message-to-parent-window-from-iframe.md)

#### Laravel
- [Append computed Eloquent model properties to JSON responses](notes/laravel/append-computed-eloquent-properties-to-json-response.md)
- [Append query parameters to pagination links](notes/laravel/append-query-parameters-in-pagination-links.md)
- [Create model, controller, and migration with one artisan command](notes/laravel/create-model-controller-migration.md) 
- [Run test without firing events](notes/laravel/run-test-without-events.md)
- [Turn off exception handling in tests](notes/laravel/turn-off-exceptions-in-laravel-tests.md)

#### MongoDB
- [Clear shell with `cls` command](notes/mongodb/clear-mongodb-shell.md)
- [Dump database to archive](notes/mongodb/dump-database-to-archive.md)

#### MySQL
- [Dump database without locking](notes/mysql/dump-database-without-blocking-writes.md)
- [Use `group_concat` to concatenate group results into a single string](notes/mysql/use-group-concat-to-group-results.md)
- [Perform case-sensitive string comparison with `BINARY` keyword](notes/mysql/perform-case-sensitive-comparison-with-binary.md)
- [See system configuration values](notes/mysql/see-configuration-values.md)
- [See the schema of a table](notes/mysql/see-schema-with-describe.md)
- [Show privileges for user](notes/mysql/show-privileges-for-user.md)

#### Networking
- [Filter Wireshark traffic by an IP address source](notes/networking/filter-wireshark-by-ip-source.md)
- [Use `dig` to query DNS information](notes/networking/use-dig-to-complement-nslookup.md)
- [Set DNS server for dig command](notes/networking/set-dns-server-for-dig-command.md)

#### Node
- [Inspect large objects](notes/node/inspect-large-objects.md)
- [List all globally installed NPM packages](notes/node/list-globally-installed-packages-npm.md)
- [Pass data to all views in Express with `res.locals` object](notes/node/pass-data-to-all-views-with-locals.md)

#### Numpy 
- [Transpose a numpy array (matrix) with `.T`](notes/numpy/transpose-matrix.md)

#### PHP
- [Assign many variables from an array with `list`](notes/php/assign-many-variables-from-array.md)
- [Build http query string from an array with `http_build_query`](notes/php/build-http-query-from-array.md)
- [Call function on script exit with `register_shutdown_function`](notes/php/call-function-on-script-exit.md)
- [Compact variables into an array](notes/php/compact-variables-into-array.md)
- [Declare nullable types](notes/php/declare-nullable-types.md)

#### PHPUnit
- [Set a default test suite](notes/phpunit/set-default-test-suite.md)
- [Set constants in config file](notes/phpunit/set-constants-in-config.md)
- [Use data providers to provide variations on input](notes/phpunit/use-data-providers.md)

#### Python
- [Extend behavior of functions with decorators](notes/python/change-function-behavior-with-decorators.md)
- [Filter a list with list comprehension](notes/python/filter-list-with-comprehension.md)
- [Unpack sequences and collections with star operator](notes/python/unpack-sequence-with-star-operator.md)
- [Use union type hints](notes/python/use-union-type-hints.md)

#### React
- [Use class properties to simplify handler functions](notes/react/use-class-properties-to-simplify-handlers.md)
- [Run cleanup function with `useEffect`](notes/react/run-cleanup-function-with-useeffect.md)

#### Rust
- [Format string output](notes/rust/format-string-output.md)
- [Use `rustup` to manage installed versions of Rust](notes/rust/use-rustup-manage-versions.md)

#### SQLite 
- [List tables and show schema from cli](notes/sqlite/list-tables-and-show-schema.md)

#### SQL Server 
- [Hash values in SQL Server](notes/sql-server/hash-values-in-sql-server.md)
- [Parse string to date](notes/sql-server/parse-string-to-date.md)

#### Theory
- [Use CAP Theorem to guide database choices](notes/theory/use-cap-theorem.md)

#### Tmux 
- [Zoom a panel to full terminal size](notes/tmux/zoom-panel-to-full-size.md)

#### Unix
- [Add a user to a group](notes/unix/add-user-to-group.md)
- [Base64 encode/decode data with `base64`](notes/unix/base64-encode-decode.md)
- [Check disk usage with `du`](notes/unix/check-disk-usage-with-du.md)
- [Check file mime type with `file` command](notes/unix/check-file-mimetype.md)
- [Compress a directory with `tar`](notes/unix/compress-directory-tar.md)
- [Convert text files from one character set to another with `iconv`](notes/unix/convert-text-file-character-set.md)
- [Forward SSH Agent with connection with `-A` flag](notes/unix/forward-ssh-agent-with-connection.md)
- [Peek at just headers of CSV file](notes/unix/peek-csv-headers.md)
- [Print sorted disk usage across device](notes/unix/print-sorted-disk-usage.md)
- [Schedule a cron job to run every X minutes](notes/unix/schedule-cron-every-x-minutes.md)
- [See differences between files with `diff`](notes/unix/see-file-differences-with-diff.md)
- [See list of files opened by processes with `lsof`](notes/unix/see-files-opened-by-process.md)
- [Test headers with `curl`](notes/unix/test-headers-with-curl.md)
- [Use `dig` to query DNS information](notes/unix/use-dig-to-complement-nslookup.md)

#### Vagrant
- [Show list of environments](notes/vagrant/show-all-vagrant-environments.md)

#### Video
- [Convert an mp4 to a gif with ffmpeg](notes/video/convert-mp4-to-gif.md)
- [Cut a clip from a video with ffmpeg](notes/video/cut-a-clip-from-video.md)
- [Remove audio from video with ffmpeg `-an`](notes/video/remove-audio-from-video-with-ffmpeg.md)

#### Vim
- [Edit file in new tab](notes/vim/edit-file-in-new-tab.md)
- [Delete without overwriting yanked text](notes/vim/delete-without-overwriting-yanked-text.md)
- [Find current word forward or back](notes/vim/find-current-word-forward-backward.md)
- [Increment and decrement numbers](notes/vim/increment-decrement-numbers.md)
- [Lowercase a series of words](notes/vim/lowercase-series-of-words.md)
- [Open a file from filename or path in source code](notes/vim/open-file-from-filename-in-source.md)
- [Open a file from netrw in new tab](notes/vim/open-file-from-netrw-in-new-tab.md)
- [Open `fzf` result in new tab](notes/vim/open-fzf-result-in-new-tab.md)
- [See list of suggested completions for current word](notes/vim/see-completion-suggestions-for-current-word.md)
- [Set the color scheme](notes/vim/set-color-scheme-in-vim.md)


