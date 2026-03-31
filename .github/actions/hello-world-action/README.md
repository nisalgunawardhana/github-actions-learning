# Hello World Action

A simple, reusable GitHub Action that greets users with customizable greeting styles.

## Usage

### Basic Usage
```yaml
- uses: ./.github/actions/hello-world-action@v1
```

### With Inputs
```yaml
- uses: ./.github/actions/hello-world-action@v1
  with:
    name: 'Alice'
    greeting-style: 'friendly'
```

## Inputs

### `name`
**Optional** The name to greet. Default: `'World'`

### `greeting-style`
**Optional** Style of greeting. Options: `friendly`, `formal`, `casual`. Default: `'friendly'`

## Outputs

### `greeting-message`
The generated greeting message.

### `timestamp`
When the greeting was generated (ISO 8601 format).

## Examples

### Friendly Greeting
```yaml
- uses: ./.github/actions/hello-world-action@v1
  with:
    name: 'Developer'
    greeting-style: 'friendly'
  # Output: Hello, Developer! 👋 Welcome!
```

### Formal Greeting
```yaml
- uses: ./.github/actions/hello-world-action@v1
  with:
    name: 'Team'
    greeting-style: 'formal'
  # Output: Good day, Team! It is a pleasure to meet you.
```

### Casual Greeting
```yaml
- uses: ./.github/actions/hello-world-action@v1
  with:
    name: 'Friends'
    greeting-style: 'casual'
  # Output: Hey Friends! What's up?
```

## Accessing Outputs
```yaml
- uses: ./.github/actions/hello-world-action@v1
  id: greet
  with:
    name: 'User'

- name: Use outputs
  run: |
    echo "Greeting: ${{ steps.greet.outputs.greeting-message }}"
    echo "Time: ${{ steps.greet.outputs.timestamp }}"
```

## Challenge Tasks Covered
This action fulfills **Challenge 3: Create a Custom Action** by:
- ✅ Creating custom action structure in `.github/actions/`
- ✅ Defining inputs and outputs in `action.yml`
- ✅ Using composite action with shell steps
- ✅ Creating reusable workflow components
- ✅ Including documentation for usage
