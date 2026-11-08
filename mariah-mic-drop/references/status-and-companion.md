# Status and companion work

A voice-led workroom can answer “where are we?” and coordinate with a configured companion without making the user learn a private command name. Run this branch when requested, not on every voice turn.

## A requested status page

Use an existing status script or connected task feed when configured. Otherwise gather from accessible task lists, run records and the current conversation. Say what sources were unavailable; never fill missing counts with guesses.

Keep a stable page with these sections, omitting no section silently: needs the user; their relevant words and decisions; broken; running; done since the last look; work log; parked work; companion inbox; news when supplied; and one clearly marked proposed addition if supported. Empty or unavailable sections get that label. Local config can map the names and data contracts to an existing workflow.

Retain exact script counts and source ages. Distinguish an assistant's completion claim from checked completion, and a stale feed from current evidence. Show the full requested page and link the saved copy. Use a usage chart only when the underlying data and chart method are available; never fabricate progress, time, cost or meter movement.

A proposed addition needs a source and remains a proposal. It does not authorize action. Do not start persistent user-message logging, monitoring or a recurring job as a hidden side effect of a status request. A legacy command may have its own explicit lifecycle; preserve that command and explain the distinction.

## A configured companion

A companion is another assistant or workspace reached by an existing supported bridge. Read its configured route and permissions before using it. With no companion configured, say so and continue the work that can be done here.

For a read request, match replies to their originating questions and show what is answered or waiting, with source age. For an authorized send, stage the exact question and necessary context, deliver through the supported route, and distinguish staged, delivered and answered. A reminder or doorbell is only a notification; it does not grant more authority.

Changes to companion instructions or scheduled tasks are separate changes with their own approval and verification. Preserve originals, report the saved result and test a schedule in its real execution environment before calling it set up. This skill does not authorize sending private information to another account or service.
