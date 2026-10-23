Copy into the ROOT of your Jekyll repo, keeping folder names.

_includes/sidebar-left.html        REPLACE your current file (inner-pages already calls it)
_includes/post-list.html           NEW  one list used by Articles and Learning Center
_includes/lc-topic.html            NEW  list for one Learning Center topic
_includes/lc-related.html          NEW  "Related reading" box (series.html already calls it)
_data/sidebar.yml                  NEW  sidebar links, edit here to change them
articles.html                      REPLACE your current Articles page (permalink /monkeyhub/articles_news/)
learning-center.html               REPLACE your current Learning Center page
topics/*.html                      NEW  six topic pages
_posts/learning_center/*.md        NEW  WCAG 2.1 vs 2.2 guide
_templates/                        reference only, do not copy into the site

Do not keep two files with the same permalink. If your Articles page lives somewhere
else (for example monkeyhub/articles.html), replace that file instead of adding articles.html.
