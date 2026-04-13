# Migrating a legacy Java Android codebase to Kotlin

Most legacy Android migrations fail when teams treat them as a language rewrite instead of a delivery strategy.

The real question is not whether Kotlin is better than Java. It is how to move toward Kotlin without freezing feature work, exhausting reviewers, or making release quality worse for six months. Teams that succeed usually treat migration as a sequence of compounding improvements rather than a heroic one-time effort.

The first step is to choose leverage points. New features, high-change modules, and bug-prone surfaces are better migration candidates than cold stable areas. If a screen already needs product work, that is often the right moment to move some surrounding Java into Kotlin as part of the same change. This keeps the migration attached to business value.

The second step is to define style and interoperability rules early. Mixed Java and Kotlin codebases become messy quickly when nullability, extension usage, coroutine patterns, and testing style are inconsistent. Teams need a shared baseline before the codebase becomes half-migrated and harder to reason about than before.

The third step is to protect review quality. Large migration pull requests create fatigue and invite rubber-stamping. Smaller slices with clear architectural intent work better. Reviewers should be able to see whether the change reduced complexity, improved state handling, or made testing easier. Otherwise migration becomes cosmetic churn.

Finally, measure the migration by outcomes, not file counts. Crash trends, development speed, onboarding clarity, and release confidence are better indicators than the percentage of files converted. Kotlin is valuable because it can help teams ship safer and move faster, not because it changes the extension on a source file.
