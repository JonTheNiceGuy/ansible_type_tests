# Ansible Value Tests

I write a lot of multi-line, complex `set_fact` and `vars` statements in Ansible.

Typically by the time I come to *use* those values, I've long-since forgotten what format
I was expecting.

Thus `is_a(n?)_(boolean|dict|float|list|string|integer).yml` was born.

These are Ansible Tasks, meant to be used to check whether the value you just passed it
was actually a value of that type... or not.

In this repo is `TEST_ME.yml` which positively runs all of these tests, and should pass
them all. I've not written a test for failing ones as yet - but it *should* come.
