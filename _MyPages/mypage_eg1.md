---
layout: page
title: Page 1
order: 10
permalink: /MyPages/
---
{% include toc.html %}  

## Paragraphs and Line Breaks

A paragraph is simply one or more consecutive lines of text, separated by one or more blank lines. (A blank
line is any line that looks like a blank line — a line containing nothing but spaces or tabs is
considered blank.) Normal paragraphs should not be indented with spaces or tabs.

The implication of the "one or more consecutive lines of text" rule is that Markdown supports "hard-wrapped”
text paragraphs. This differs significantly from most other text-to-HTML formatters (including Movable
Type's "Convert Line Breaks” option) which translate every line break character in a paragraph into a `<br>` tag.

When you do want to insert a `<br>` break tag using Markdown, you end a line with two or more spaces, then type return.

Yes, this takes a tad more effort to create a `<br>`, but a simplistic "every line break is a `<br>`” rule
wouldn't work for Markdown. Markdown's email-style blockquoting and multi-paragraph list items work best —
and look better — when you format them with hard breaks.

## Blockquotes

Markdown uses email-style > characters for blockquoting. If you're familiar with quoting passages of text
in an email message, then you know how to create a blockquote in Markdown.

## Subheading 1

Contents for subheading 1 added here

## Subheading 2

Contents for subheading 2 added here


<!-- {% assign collection = page.collection %}
{{collection}}

{% assign docs = site.[collection] %}

{% if docs %}
    {% assign sorted_docs = docs | sort:"order","last" %}

    {% for document in sorted_docs %}
                    	{% if document.title != null %}
                               {% assign subheadings = document.subheadings %}
                               {{document.title}}
                               {{subheadings}}

                               {% if subheadings.size != 0 %}
                                      {{subheadings.size}}

                                      {% for subheading in subheadings %}
                                        {{subheading.title }}
                                      {% endfor %}

                               {% endif %}
                       {% endif %}
    {% endfor %}
{% endif %} -->
