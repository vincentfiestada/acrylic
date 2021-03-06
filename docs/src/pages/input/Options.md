## Options

An **Options Group** lets the user pick from a few available choices.

```jsx
render(() => (
	<>
		<Options label="Options" required selection={2} onSelect={val => alert(val)}>
			<Option value={1} label="Option" />
			<Option value={2} label="Disabled" disabled/>
			<Option value={3} label="Primary" variant="primary"/>
			<Option value={4} label="Success" variant="success"/>
			<Option value={5} label="Warning" variant="warning"/>
			<Option value={6} label="Danger" variant="danger"/>
		</Options>
		<Options label="Invalid" invalid comment="This field has an error">
			<Option value={1} label="Acamar" />
			<Option value={2} label="Acubens" />
			<Option value={3} label="Polaris" />
			<Option value={4} label="Pollux" />
			<Option value={5} label="Sirius" />
		</Options>
		<Options label="Success" variant="success" comment="This field is correct">
			<Option value={1} label="Acamar" />
			<Option value={2} label="Acubens" />
			<Option value={3} label="Polaris" />
			<Option value={4} label="Pollux" />
			<Option value={5} label="Sirius" />
		</Options>
	</>
))
```

If the field is read-only, only the label of the selected value is rendered.

```jsx
render(() => (
	<>
		<Options readOnly selection={1} label="Options">
			<Option value={1} label="Acamar" />
			<Option value={2} label="Acubens" />
			<Option value={3} label="Polaris" />
			<Option value={4} label="Pollux" />
			<Option value={5} label="Sirius" />
		</Options>
		<Options readOnly selection={2} label="Invalid" invalid comment="This field has an error">
			<Option value={1} label="Acamar" />
			<Option value={2} label="Acubens" />
			<Option value={3} label="Polaris" />
			<Option value={4} label="Pollux" />
			<Option value={5} label="Sirius" />
		</Options>
		<Options readOnly selection={3} label="Success" variant="success" comment="This field is correct">
			<Option value={1} label="Acamar" />
			<Option value={2} label="Acubens" />
			<Option value={3} label="Polaris" />
			<Option value={4} label="Pollux" />
			<Option value={5} label="Sirius" />
		</Options>
	</>
))
```

###### Options

- [`Options`](/wiki/modules/_components_input_options_.html)
- [`Option`](/wiki/modules/_components_input_options_.html#option)
