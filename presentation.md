%title: React's introduction
%author: godu
%date: 2015-12-18

-> React's introduction <-
==========================

\- Virtual dom
\- diff algorithm
\- React Component
\- Dumb & Smart component
\- Alteratives

-------------------------------------------------

-> Virtual dom <--
==================

{                           |
  *type: 'h1'*,               | < *h1* >
  props: {                  |
    *id: 'title'*,            |  *id="title"*
    children: *'Title'*       |     *Title*
  }                         |
}                           | </h1>

-------------------------------------------------

-> Virtual dom <--
==================

{                           |
  *type: 'header'*,           | < *header*
  props: {                  |
    *id: 'header'*,           |  *id="header"*
    children: {             | >
      *type: 'h1'*,           |   < *h1* >
      props: {              |
        children: *'Title'*   |     *Title*
      }                     |
    }                       |   </h1>
  }                         | </header>
}                           |

-------------------------------------------------

-> Virtual dom <--
==================

{
  *type: 'h1'*,
  props: {
    *id: 'title'*,
    children: *'Title'*
  }
}

<html>
  <body>
  </body>
</html>


▛▀▀▀▀▀▀▀▀▀▜
▌rectangle▐
▙▄▄▄▄▄▄▄▄▄▟