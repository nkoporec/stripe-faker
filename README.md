# stripe-faker

A CLI tool to bulk auto-generate Stripe entities (users, products, subscription)

# Getting Started

Install the command-line tool:

```
cargo install
```

## Commands at a glance

| command                | description                                                                   |
| ---------------------- | -----------------------------------------                                     |
| create-users           | Create dummy users (with optional attached subscription and a payment method) |

## TODO

 - [ ] Auto-generate products
 - [ ] Auto-generate prices

# Usage

You need a Stripe secret key, the key can be set as a `STRIPE_SECRET_KEY` environoment variable or passed to the cli as `--secret_key=[KEY]` argument.

<hr>

#### `stripe-faker --help`

Show a list of options and commands for the <abbr title="Command Line Interface">CLI</abbr>.

<hr>

#### `stripe-faker create-users {number_of_users}`

Create a N amount of users on Stripe. The names and email are randomly generated.

#### Optional arguments:

 ##### --subscription_create [name]
  Creates a new subscription product with [name] and a monthly price of 10$, all generated users are automatically subscribed to it.
  
 ##### --card [card_number]
  Attaches a credit card with [card_number] with CVC and expire date set to all generated users.
