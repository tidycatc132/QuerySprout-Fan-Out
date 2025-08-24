# Query Fan-Out Analysis Tool

A powerful Streamlit application that uses Google's Query Fan-Out methodology to help you optimize content for AI-powered search results and Google AI Overviews.

## Features

### Two Analysis Modes:

1. **New Content Planning** 
   - Generate query variants using Google's Fan-Out system
   - Plan comprehensive content strategies
   - Identify content gaps before writing
   - Create topic clusters and content hierarchies

2. **Optimize Existing Content**
   - Analyze any URL for optimization opportunities
   - Compare against target keywords
   - Identify missing query coverage
   - Get specific rewrite recommendations
   - Competitive analysis against other URLs

## Query Fan-Out Methodology

Based on [Google's Query Fan-Out System], this tool generates 7 types of query variants:

- **Equivalent Queries** - Alternative ways to ask the same question
- **Follow-up Queries** - Logical next questions
- **Generalization Queries** - Broader topic versions
- **Canonicalization Queries** - Standardized search terms
- **Entailment Queries** - Logically implied questions
- **Specification Queries** - More detailed versions
- **Clarification Queries** - Intent clarification

## Setup Instructions

### Prerequisites

- Python 3.8 or higher
- Gemini API key from [Google AI Studio](https://makersuite.google.com/app/apikey)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/query-fanout-tool.git
   cd query-fanout-tool
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Set up your Gemini API key:
   
   **Option 1: Environment Variable**
   ```bash
   export GEMINI_API_KEY="your-api-key-here"
   ```
   
   **Option 2: Streamlit Secrets**
   Create `.streamlit/secrets.toml`:
   ```toml
   GEMINI_API_KEY = "your-api-key-here"
   ```

4. Run the application:
   ```bash
   streamlit run app.py
   ```

## How to Use

### For New Content Planning:

1. Select "New Content Planning" mode
2. Enter your target queries (one per line)
3. Configure analysis settings:
   - Choose query variant types to generate
   - Select optimization target (AI Overviews, AI Mode, or Both)
   - Set analysis depth
4. Click "Run Query Fan-Out Analysis"
5. Review recommendations and download report

### For Existing Content Optimization:

1. Select "Optimize Existing Content" mode
2. Enter your content URL
3. Provide primary keyword and additional keywords
4. Optionally add competitor URLs for comparison
5. Configure analysis options
6. Click "Analyze & Optimize Content"
7. Implement the specific recommendations provided

## Configuration Options

### Analysis Settings:
- **Gemini Model**: Choose between Flash (faster) or Pro (more capable)
- **Analysis Depth**: Basic, Standard, or Comprehensive
- **Optimization Target**: 
  - AI Overviews (quick answers)
  - AI Mode (complex query fan-out)
  - Both (comprehensive optimization)

### Advanced Features:
- Entity relationship mapping
- Cross-variant verification
- Schema markup recommendations
- Competitive analysis
- Snippet optimization
- People Also Ask optimization

## Output Reports

The tool provides detailed reports including:

- Query variant generation for all selected types
- Content architecture recommendations
- Specific optimization actions (immediate, short-term, long-term)
- Content rewrite examples
- Schema markup suggestions
- Success metrics and KPIs

Reports can be exported in:
- Markdown format (for documentation)
- JSON format (for programmatic use)
- Full report format (comprehensive analysis)

## 📄 License

This project is licensed under the MIT License.

## For Best Results

### New Content Planning:
- Start with 5-10 core queries
- Include both broad and specific queries
- Consider user intent variations
- Think about the customer journey

### Content Optimization:
- Use your main target keyword
- Include 3-5 related keywords
- Add 2-3 competitor URLs for comparison
- Ensure URLs are publicly accessible
- Review all recommendations before implementing

## Troubleshooting

**Content fetching fails:**
- Check if the URL is publicly accessible
- Verify the site doesn't block web scrapers
- Try a different URL from the same domain

**Gemini API errors:**
- Verify your API key is valid
- Check API quotas and limits
- Try using a different model (Flash vs Pro)

**Analysis takes too long:**
- Reduce analysis depth
- Use fewer query variants
- Choose Flash model for faster processing

---

**Note**: This tool requires a valid Gemini API key. Ensure you have the necessary API credentials before use.
