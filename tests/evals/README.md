# Pydantic Evals Tests

This directory contains test files for the `pydantic_evals` package.

## Running Tests

To run all tests in this folder, use the following command:

```bash
uv run pytest tests/evals/ -v
```

This command will execute all test cases found in the `tests/evals` directory with verbose output, allowing you to see detailed results for each test.

## Test Files

The test suite includes:

- `test_dataset.py` - Tests for dataset functionality
- `test_evaluator_base.py` - Tests for base evaluator classes
- `test_evaluator_common.py` - Tests for common evaluator functionality
- `test_evaluator_context.py` - Tests for evaluator context
- `test_evaluator_spec.py` - Tests for evaluator specifications
- `test_evaluators.py` - Tests for evaluator implementations
- `test_llm_as_a_judge.py` - Tests for LLM-based evaluation
- `test_otel.py` - Tests for OpenTelemetry integration
- `test_render_numbers.py` - Tests for number rendering
- `test_reporting.py` - Tests for evaluation reporting
- `test_reports.py` - Tests for report generation
- `test_utils.py` - Tests for utility functions

## Running Specific Tests

To run a specific test file:

```bash
uv run pytest tests/evals/test_dataset.py -v
```

To run a specific test function:

```bash
uv run pytest tests/evals/test_dataset.py::test_dataset_init -v
```

## Additional Options

- Add `-s` to see print statements: `uv run pytest tests/evals/ -v -s`
- Add `--pdb` to drop into debugger on failures: `uv run pytest tests/evals/ -v --pdb`
- Add `-k <pattern>` to run tests matching a pattern: `uv run pytest tests/evals/ -v -k "dataset"`
