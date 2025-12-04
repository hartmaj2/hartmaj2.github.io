---
layout: default
title: Čtenářský deník
permalink: /reading-list/
navbar_order: 0
---

<h1>Čtenářský deník</h1>

<div class="posts-list">
    <ul>
        {% for book in site.books %}
        <li class="book-item">
            <div class="book-main">
                <a href="{{ book.url | relative_url }}">{{ book.title }}</a>
                {% if book.author %}
                    – {{ book.author }}
                {% endif %}
            </div>

            <div class="book-meta">
                {% if book.started %}
                    <span><em>📘 začteno: {{ book.started | date: "%-d. %-m. %Y" }}</em></span>
                {% endif %}

                {% if book.finished %}
                    <span><em>📗 dočteno: {{ book.finished | date: "%-d. %-m. %Y" }}</em></span>
                {% endif %}
            </div>
        </li>

        {% endfor %}
    </ul>
</div>
