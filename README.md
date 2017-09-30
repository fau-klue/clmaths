[![Build Status](https://travis-ci.org/martialblog/clmaths.svg?branch=master)](https://travis-ci.org/martialblog/clmaths)

# Mathematics for Computational Linguistics

This is a small collection of basic mathematics for your off-the-shelf Computer Linguist.

https://martialblog.github.io/clmaths/

# Development and Contributing

This website is generated using Ruby Jekyll: https://jekyllrb.com/

So that means you will have to install Ruby and Bundler on your system.

Installation of dependencies:

```bash
bundle install --path=.bundle
```

Running the local Jekyll server:

```bash
bundle exec jekyll serve
```

The site can then be reached at: http://localhost:4000/clmaths/

## Testing

To run the tests in the Rakefile:

```bash
bundle exec rake test
```

## Mathematical Notation

For the mathematical notation we use [MathJax](https://www.mathjax.org/). Formulas can be written in TeX, see the MathJax documentation for details.

## Code Snippets

To include Code examples we (for far) use JavaScript and R playgrounds (fiddle), so that the code can directly be included into the courses.

    - https://jsfiddle.net/
    - http://www.r-fiddle.org/
