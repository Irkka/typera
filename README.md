# typera(pronounced: typerä) - *The stupid typography library*

Typera is your one-stop solution to typeface and typesetting problems in your websites. Instead of polluting your markup with alien classes, typera offers a framework to extend your own classes with pre-defined typography solutions - thus keeping your markup cleaner and your SassScript more DRY. It also aims to follow the best practices proposed by The Sass Way and some of my personal views of how things should be done. For example, styles/properties should not be assigned to elements but to classes instead, unless they're direct descendants to the article or any arbitrary text type class, in which case it naturally makes sense and doesn't provoke unintended styling clashes. This gives exact control over the site's typography settings and enables quick changes, should the context call for it.

Typera also build upon Ross Penman's library for easy Google Web Font importing and typography examples provided by thoughtbot's Refills.

## Example usage

```
@import 'typera';

.blog-post {
  @include article('Geometric');
}
```
