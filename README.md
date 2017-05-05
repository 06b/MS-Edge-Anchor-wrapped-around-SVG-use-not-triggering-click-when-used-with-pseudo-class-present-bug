# MS Edge Anchor wrapped around SVG <use> not triggering click when used with pseudo-class present

 * Test case (1) - Control.
 * Test case (2) - Reversed SVG usage of test case (1) in the event issue is related to the SVG used.
 * Test case (4,6) are based off of the test case (2).
 * Test cases (3,5) are based off of the test case (1).

---

 * Test case (1) - Embedded and linked SVG with no pseudo-class present working as expected.
 * Test case (2) - For some reason parts of the SVG within the linked SVG fails however that is not the reason for this bug.
 * Test case (3) - Pseudo-class present and applied to markup. Fails test - Bug
 * Test case (4) - Pseudo-class present and applied to markup. Fails test - Bug
 * Test case (5) - Pseudo-class present and not applied to markup. Fails test - Bug
 * Test case (6) - Pseudo-class present and not applied to markup. Fails test - Bug

## Credit

 * SVG_logo.svg - https://commons.wikimedia.org/wiki/File:SVG_logo.svg
 * svg-logo-h.svg - https://www.w3.org/2009/08/svg-logos.html

## Notes

SVG logos which were embedded and linked were optimized via SVGO and then manually edited for test cases to help make sure test case is reduced.

Workarounds included for failing test cases (2,3,4,5,6).

---
 * Test case (7) - Shows issue with workaround, that using <code>pointer-events: none</code> causes hover not to apply - however that is not the reason for this bug.
* Workaround included for test case (7) however this increases css specificity and is troublesome. Test case (7) is only included so if someone uses any of the workarounds for the failing test cases (2,3,4,5,6) they will know the side effects.
 
