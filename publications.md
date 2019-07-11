---
title: "Publications"
date: 2019-07-09 09:00:05
categories: [general]
tags: [general]
layout: page
permalink: /publications/
---

<script>
coming soon :-)

$.get('https://graz.pure.elsevier.com/en/persons/michael-spitzer/publications/?format=rss', function (data) {
    $(data).find("item").each(function () { // or "item" or whatever suits your feed
        var el = $(this);

        console.log("------------------------");
        console.log("title      : " + el.find("title").text());
        console.log("link     : " + el.find("link").text());
        console.log("description: " + el.find("description").text());
    });
});
</script>
