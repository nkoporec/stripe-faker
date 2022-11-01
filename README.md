# stripe-faker

A CLI tool to bulk auto-generate Stripe entities (users, products, subscription)

# Getting Started

Install the command-line tool:

```
cargo install
```

## Commands at a glance

| command                | description                                                                 |
| ---------------------- | -----------------------------------------                                   |
| create-users           | Create dummy users (with optional attached subscription and payment method) |

# Usage

## `stripe-faker --help`

Show a list of options and commands for the <abbr title="Command Line Interface">CLI</abbr>.


## `stripe-faker create-users {number_of_users}`

Create a N amount of users on Stripe.

```
stripe-faker create-users 50
```
