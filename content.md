# Heading

This is an interactive documentation for research and work process.
---
{
    "name": "data",
    "children": [
        {
            "name": "L0",
            "level": 0,
            "children": [
                {
                    "name": "1",
                    "type": "topic",
                    "content": "Topic",
                    "imports": []
                },
                {
                    "name": "2",
                    "type": "process",
                    "content": "Process",
                    "imports": []
                },
                {
                    "name": "3",
                    "type": "question",
                    "content": "Question",
                    "imports": []
                },
                {
                    "name": "5",
                    "type": "input",
                    "content": "Input",
                    "imports": []
                },
                {
                    "name": "6",
                    "type": "result",
                    "content": "Result",
                    "imports": []
                }
            ]
        },
        {
            "name": "L1",
            "level": 1,
            "children": [
                {
                    "name": "4",
                    "type": "output",
                    "content": "Output",
                    "imports": ["data.L0.1", "data.L0.3", "data.L0.6"]
                }
            ]
        }
    ]
}
-----
# Two

This is an interactive documentation for research and work process.

---
{
    "name": "data",
    "children": [
        {
            "name": "L0",
            "level": 0,
            "children": [
                {
                    "name": "1",
                    "type": "topic",
                    "content": "Topic",
                    "imports": []
                },
                {
                    "name": "2",
                    "type": "process",
                    "content": "Process",
                    "imports": []
                },
                {
                    "name": "3",
                    "type": "question",
                    "content": "Question",
                    "imports": []
                },
                {
                    "name": "5",
                    "type": "input",
                    "content": "Input",
                    "imports": []
                },
                {
                    "name": "6",
                    "type": "result",
                    "content": "Result",
                    "imports": []
                }
            ]
        },
        {
            "name": "L1",
            "level": 0,
            "children": [
                {
                    "name": "4",
                    "type": "result",
                    "content": "Output",
                    "imports": ["data.L0.1", "data.L0.2", "data.L0.3", "data.L0.6"]
                }
            ]
        },
        {
                        "name": "L2",
            "level": 0,
            "children": [
                {
                    "name": "4",
                    "type": "result",
                    "content": "Output",
                    "imports": ["data.L0.1"]
                }
            ]
        }
    ]
}

