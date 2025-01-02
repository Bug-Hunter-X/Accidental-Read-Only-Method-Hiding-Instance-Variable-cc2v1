# Accidental Read-Only Method Hiding Instance Variable

This Ruby code example showcases a subtle but common error.  The `value` method unintentionally hides the instance variable `@value`, making it appear read-only.  The assignment `my_object.value = 20` does not update the instance variable because Ruby sees `value` as a method and not as an accessor to `@value`.