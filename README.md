# Well of Wisdom - Community Courses

Shared course library for [Well of Wisdom](https://github.com/wellofwisdom/wellofwisdom). Each folder under `courses/` holds one CC-BY course you can import into any instance with one link.

## Adding a course

1. Build and review it on any Well of Wisdom instance. Read every question and its answer.
2. Export it from the course page (includes answers).
3. Put it at `courses/<slug>/course.wow-course.json`, add a `README.md` if you like, and open a pull request.

## Importing a course

In your Well of Wisdom instance: **Courses -> Import -> Paste a shared course link** and paste the link to the file on GitHub (file page or raw). It lands as a draft to review before learners see it.

## What gets checked

`node ../wellofwisdom/scripts/validate-course.js --library courses` runs on every PR. A course needs:

- An open licence (CC-BY-4.0, CC-BY-SA-4.0 or CC0-1.0)
- Every question with its answer (export with answers included)
- Nothing lost on import (size limits, valid shapes)

See [wellofwisdom/docs/COMMUNITY-COURSES.md](https://github.com/wellofwisdom/wellofwisdom/blob/main/docs/COMMUNITY-COURSES.md) for the full spec.
