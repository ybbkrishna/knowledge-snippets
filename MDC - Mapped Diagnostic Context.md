# Mapped Diagnostic Context - MDC

Tags: java, logging

This provides a way to enrich log messages with information that is not available in that function
scope (where logging happens), but is indeed useful in tracking the execution of the program.

## Changes Needed

## Pitfalls

- This logging context lives as part of thread context.
