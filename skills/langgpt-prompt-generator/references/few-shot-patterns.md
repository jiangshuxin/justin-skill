# Few-shot Example Patterns

## Pattern Types

### 1. Q&A Pattern
适用于问答类助手，展示如何处理不同类型的问题。

```markdown
### Example 1
User: What is the capital of France?
Assistant: The capital of France is Paris. It is located in the north-central part of the country and has been the political center since the 5th century.

### Example 2
User: Can you explain quantum computing in simple terms?
Assistant: Quantum computing uses quantum mechanics principles to process information. Unlike classical computers that use bits (0 or 1), quantum computers use qubits which can exist in multiple states simultaneously. This allows them to solve certain complex problems much faster than traditional computers.

### Example 3
User: How do I bake a chocolate cake?
Assistant: Here's a simple chocolate cake recipe:
Ingredients:
- 2 cups flour
- 2 cups sugar
- 3/4 cup cocoa powder
- 2 eggs
- 1 cup milk
- 1/2 cup vegetable oil

Instructions:
1. Preheat oven to 350°F (175°C)
2. Mix dry ingredients in a large bowl
3. Add eggs, milk, and oil, stir until smooth
4. Pour into greased 9x13 inch pan
5. Bake for 30-35 minutes
```

### 2. Task Execution Pattern
适用于任务执行类助手，展示完整的工作流程。

```markdown
### Example 1
User: Summarize the following text in 3 bullet points: "Machine learning is a subset of artificial intelligence that enables systems to learn from data without being explicitly programmed. It involves algorithms that improve automatically through experience. Common applications include image recognition, natural language processing, and predictive analytics."
Assistant:
- Machine learning is an AI subset that enables systems to learn from data
- Algorithms improve automatically through experience
- Applications include image recognition, NLP, and predictive analytics

### Example 2
User: Extract all email addresses from this text: "Contact us at support@example.com or sales@company.org for more information. Our team at tech@startup.io is also available."
Assistant: support@example.com, sales@company.org, tech@startup.io

### Example 3
User: Rewrite this paragraph to be more professional: "Hey, I want to talk about the project thing. Let me know when you can."
Assistant: I would like to discuss the project. Please let me know your availability for a meeting at your earliest convenience.
```

### 3. Creative Generation Pattern
适用于创意生成类助手，展示风格和格式要求。

```markdown
### Example 1
User: Write a haiku about nature
Assistant:
Morning light breaks through
Dew drops on leaves sparkle bright
Nature breathes anew

### Example 2
User: Create a product tagline for a smart watch
Assistant: Time on Your Wrist, Life at Your Fingertips

### Example 3
User: Generate a 5-sentence story about a lost cat
Author: The small orange kitten sat by the busy road, its whiskers trembling. Cars rushed by, their wheels turning in a blur of motion and noise. A little girl spotted him from her window and rushed outside with gentle hands. She scooped him up, whispering comforting words as she carried him home. Safe and warm, the kitten purred, finally found.
```

### 4. Code Generation Pattern
适用于代码生成类助手，展示不同编程场景。

```markdown
### Example 1
User: Write a Python function to calculate factorial
Assistant:
```python
def factorial(n):
    """Calculate the factorial of a positive integer."""
    if n < 0:
        raise ValueError("Factorial is not defined for negative numbers")
    if n == 0 or n == 1:
        return 1
    return n * factorial(n - 1)
```

### Example 2
User: Create a REST API endpoint in Express.js that returns user data
Assistant:
```javascript
const express = require('express');
const router = express.Router();

router.get('/users/:id', async (req, res) => {
    try {
        const user = await User.findById(req.params.id);
        if (!user) {
            return res.status(404).json({ error: 'User not found' });
        }
        res.json(user);
    } catch (error) {
        res.status(500).json({ error: 'Internal server error' });
    }
});

module.exports = router;
```

### Example 3
User: Write SQL query to find top 5 customers by order count
Assistant:
```sql
SELECT c.customer_id, c.name, COUNT(o.order_id) as order_count
FROM customers c
LEFT JOIN orders o ON c.customer_id = o.customer_id
GROUP BY c.customer_id, c.name
ORDER BY order_count DESC
LIMIT 5;
```
```

### 5. Analysis Pattern
适用于分析类助手，展示分析方法论。

```markdown
### Example 1
User: Analyze this customer feedback: "The product is great but shipping was slow and expensive."
Assistant:
**Positive Aspects:**
- Product quality (customer satisfaction with the item itself)

**Areas for Improvement:**
- Shipping speed (delivery time)
- Shipping cost (pricing issue)

**Recommendations:**
- Evaluate shipping partners for faster options
- Consider offering free shipping for orders above a threshold
- Provide shipping cost transparency upfront

### Example 2
User: Compare Python and JavaScript for data analysis
Assistant:
**Python Strengths:**
- Extensive data science libraries (pandas, NumPy, scikit-learn)
- Better performance for numerical computations
- Strong statistical and scientific computing ecosystem

**JavaScript Strengths:**
- Direct browser integration for web-based visualization
- Asynchronous processing capabilities
- Growing data libraries (D3.js, Observable Plot)

**Conclusion:**
Python remains the preferred choice for traditional data analysis, while JavaScript excels for web-based interactive visualizations and real-time dashboards.

### Example 3
User: Evaluate the risk of this investment: $10,000 in a tech startup
Assistant:
**Risk Assessment:**

High Risk Factors:
- Startup failure rate (~90% within first 5 years)
- Market uncertainty in tech sector
- Limited diversification with single investment

Potential Rewards:
- High return potential if successful (10-100x possible)
- Early access to innovative technology
- Possible tax benefits (depending on jurisdiction)

**Recommendation:**
Only invest if you can afford total loss and the startup shows strong metrics: clear business model, experienced team, and market validation. Consider diversifying across multiple startups if possible.
```

## Few-shot Best Practices

1. **Diversity**: Include varied examples covering different scenarios
2. **Realism**: Use realistic inputs and outputs
3. **Clarity**: Ensure examples are self-contained and easy to understand
4. **Consistency**: Maintain consistent format across all examples
5. **Edge Cases**: Include at least one example handling edge cases or errors
6. **Length**: Balance brevity with necessary detail in each example

## Customizing for Your Domain

When adapting these patterns:

1. **Identify your core task type** (Q&A, analysis, generation, etc.)
2. **Select the matching pattern** from above
3. **Replace placeholder content** with domain-specific examples
4. **Adjust quantity** based on task complexity (2-4 examples is typical)
5. **Test with varied inputs** to ensure the examples effectively guide the model
