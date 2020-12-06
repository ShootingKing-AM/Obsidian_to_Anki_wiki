In any note, you can do clozes using Anki's standard syntax:  
`This is a {{c1::cloze note}}`  
However, by enabling the 'CurlyCloze' option (see [[Config]]), you have access to many easier options:

1. `This is a {cloze} note with {two clozes}`
->
`This is a {{c1::cloze}} note with {{c2::two clozes}}`
2. `This is a {2:cloze} note with {1:id syntax}`
->
`This is a {{c2::cloze}} note with {{c1::id syntax}}`
3. `This is a {2|cloze} {3|note} with {1|alternate id syntax}`
->
`This is a {{c2::cloze}} {{c3::note}} with {{c1::alternate id syntax}}`
4. `This is a {c1:cloze} note with {c2:another} type of {c3:id syntax}`
->
`This is a {{c1::cloze}} note with {{c2::another}} type of {{c3::id syntax}}`
5. `This is a {c1|cloze} note with {c2|yet another} type of {c3|id syntax}`
->
`This is a {{c1::cloze}} note with {{c2::yet another}} type of {{c3::id syntax}}`

You can also mix and match styles! Note that clozes without an id will always be assigned an id starting from 1, increasing for each new cloze:
`This is a {cloze} note with {multiple} non-id clozes, as well as {2:some clozes} with {c1|other styles}`
->
`This is a {{c1::cloze}} note with {{c2::multiple}} non-id clozes, as well as {{c2::some clozes}} with {{c1::other styles}}`