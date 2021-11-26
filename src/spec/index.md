# Fe Language Specification

<div class="warning">
  Warning: This is a work in progress document. It is incomplete and specifications aren't stable yet.
</div>

* [Notation](notation.md)
* [Lexical Structure](lexical_structure.md)
    * [Keywords](keywords.md)
    * [Identifiers](identifiers.md)
    * [Tokens](tokens.md)
* [Comments](comments.md)
* [Items](items.md)
    * [Visibility and Privacy](visibility_and_privacy.md)
    * [Functions](functions.md)
    * [Structs](structs.md)
    * [Events](events.md)
    * [Enumeration](enumeration.md)
    * [Type Aliases](type_aliases.md)
    * [Contracts](contracts.md)
* [Statements](statements.md)
    * [`pragma` Statement](statement_pragma.md)
    * [Assignment Statement](statement_assign.md)
    * [Augmenting Assignment Statement](statement_augassign.md)
    * [`const` Statement](statement_const.md)
    * [`let` Statement](statement_let.md)
    * [`revert` Statement](statement_revert.md)
    * [`return` Statement](statement_return.md)
    * [`emit` Statement](statement_emit.md)
    * [`if` Statement](statement_if.md)
    * [`for` Statement](statement_for.md)
    * [`while` Statement](statement_while.md)
    * [`break` Statement](statement_break.md)
    * [`continue` Statement](statement_continue.md)
    * [`assert` Statement](statement_assert.md)
    * [`pass` Statement](statement_pass.md)
* [Expressions](expressions.md)
    * [Call expressions](expr_call.md)
    * [Tuple expressions](expr_tuple.md)
    * [List expressions](expr_list.md)
    * [Index expressions](expr_index.md)
    * [Attribute expressions](expr_attribute.md)
    * [Name expressions](expr_name.md)
    * [Literal expressions](expr_literal.md)
    * [Arithmetic Operators](expr_arithmetic_operators.md)
    * [Comparison Operators](expr_comparison_operators.md)
    * [Boolean Operators](expr_boolean_operators.md)
    * [Unary Operators](expr_unary_operators.md)
* [Type System](type_system.md)
    * [Types](types.md)
        * [Boolean Type](boolean_type.md)
        * [Contract Type](contract_types.md)
        * [Numeric Types](numeric_types.md)
        * [Tuple Types](tuple_types.md)
        * [Array Types](array_types.md)
        * [Struct Types](struct_types.md)
        * [Enumerated Types](enumerated_types.md)
        * [Address Type](address_type.md)
        * [HashMap Type](hashmap_type.md)
        * [String Type](string_type.md)
        * [Event Types](event_types.md)
* [Data Layout](data_layout.md)
    * [Stack](stack.md)
    * [Storage](storage.md)
        * [Constant size values in storage](constant_size_values_in_storage.md)
        * [Maps in storage](maps_in_storage.md)
        * [`to_mem()` function](to_mem_function.md)
    * [Memory](memory.md)
        * [Sequence types in memory](sequence_types_in_memory.md)
        * [`clone()` function](clone_function.md)
* [Function calls](function_calls.md)