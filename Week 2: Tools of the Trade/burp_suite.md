# Burp Suite

Burp Suite is an excellent http proxy / intrusion tool. It comes in both free and paid varieties. If it's useful to your job, the paid version looks to be well worth the investment. As a hobbyist, the free edition still provides a lot of use.

The core of the program is your standard proxy. It intercepts requests and responses within scope and allows you to modify them. You can then send the intercepted requests or responses to many of the other modules.

On top of one of the most intuitive HTTP proxies I've used, the following functionality is built:

## Spider

The spider will crawl all pages in scope, prompting you for details to submit into any forms.

## Scanner (paid version)

Looks like a fairly standard vulnerability scanner. Given that it's paid only, I can't testify to how effective it is.

## Intruder

Allows you to craft HTTP requests with one or more payload sources. Entries from the payload sources are inserted into user-defined locations in each request, depending on the selected attack type. Pre-processing can be performed on the payloads, and the paid version appears to include pre-set payload lists.

## Repeater

Simply allows you to manually send and re-send HTTP requests to analyse differences between responses.

## Sequencer

Allows you to send a repeated request, collect some token such as an issued session token, and analyse its randomness.

## Decoder

A simple base64 / binary / hex encoder and hash calculator. Does what it says on the tin.

## Comparer

Provides pretty nice visual diffs between two items.

## Extender

Burp Suite has an allegedly pretty great plugin system, which I haven't yet played with. Maybe another week!
