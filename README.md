Shopify_Development_Guide:
  Introduction:
    Description: >
      This document is a complete learning and interview preparation guide for developers transitioning
      into Shopify development. It is designed for developers with React, Next.js, WordPress, or WooCommerce
      experience who need to prepare quickly for Shopify interviews while also building a strong foundation
      for on-the-job learning.
    Audience: 
      - Frontend developers (React, Next.js)
      - WordPress/WooCommerce developers
      - E-commerce engineers

  Section_1: Shopify_Overview:
    What_is_Shopify: >
      Shopify is a SaaS-based e-commerce platform that provides merchants with hosting, security,
      checkout, and payment integrations out of the box. Developers extend Shopify through themes, apps,
      APIs, and custom storefronts.
    Key_Differences_from_WooCommerce: 
      - Shopify is hosted SaaS; WooCommerce is a WordPress plugin (self-hosted).
      - Shopify manages servers and infrastructure automatically.
      - WooCommerce requires plugins and manual updates.
      - Shopify checkout is secure but restricted; WooCommerce checkout is fully customizable.

  Section_2: Shopify_Development_Areas:
    Themes:
      Description: >
        Shopify themes define the storefront look and feel.
      Technology:
        - Liquid templating
        - HTML, CSS, JavaScript
      Structure:
        - Layouts
        - Templates
        - Sections
        - Snippets
      Tools:
        - Shopify CLI
        - Dawn theme
    Apps:
      Description: >
        Apps extend Shopify’s native functionality (similar to WordPress plugins).
      Types:
        - Public Apps (listed on App Store)
        - Custom Apps (store-specific)
      Tech_Stack:
        - Node.js
        - React (Polaris + App Bridge)
        - GraphQL & REST APIs
    Storefront_API_and_Hydrogen:
      Description: >
        Hydrogen is Shopify’s React-based framework for headless storefronts.
      Uses:
        - Custom frontends with Next.js-like workflows
        - GraphQL queries to fetch products, collections, carts, and checkout
    Checkout:
      Standard: Locked and secure.
      Shopify_Plus: Checkout extensibility with UI extensions and scripts.
    APIs_and_Webhooks:
      Admin_API: >
        REST and GraphQL APIs for managing store data (products, orders, customers).
      Storefront_API: >
        GraphQL API for custom storefronts.
      Webhooks: >
        Event-based callbacks (e.g., order/create).
    Metafields:
      Description: >
        Custom fields that extend Shopify objects (products, collections, customers, orders).

  Section_3: Framing_Prior_Experience:
    Question: "You don’t have direct Shopify experience — how will you manage?"
    Answer: >
      I have strong experience in React, Next.js, and WordPress/WooCommerce e-commerce development.
      I understand core e-commerce concepts: product catalogs, carts, checkout, payments, and APIs.
      Shopify development builds on the same principles but uses its own templating system (Liquid) and APIs.
      I’ve already studied Shopify’s ecosystem, Liquid, and API structure, and I’m confident I can ramp up
      quickly while applying my prior front-end and e-commerce experience.
    Question2: "Why Shopify?"
    Answer2: >
      Shopify is one of the most scalable and widely adopted e-commerce platforms today. It allows developers
      to focus on building great user experiences instead of worrying about hosting and infrastructure.
      With Shopify Plus, headless commerce, and Hydrogen, it’s at the cutting edge of modern commerce.
      I want to bring my React/Next.js expertise into Shopify’s ecosystem.

  Section_4: Step_by_Step_Learning_Roadmap:
    Step_1: "Understand Shopify Admin and Store Basics"
    Step_2: "Install Shopify CLI and explore the Dawn theme"
    Step_3: "Learn Liquid templating basics"
    Step_4: "Build and customize Sections and Blocks"
    Step_5: "Work with Products, Collections, and Metafields"
    Step_6: "Practice with Storefront API (GraphQL)"
    Step_7: "Explore Hydrogen for headless commerce"
    Step_8: "Build a simple Shopify App with Node.js + React"
    Step_9: "Implement Webhooks for automation"
    Step_10: "Understand Checkout Extensibility (Shopify Plus)"

  Section_5: Interview_Questions_and_Answers:
    Total_Questions: 50
    Categories:
      - Conceptual (1-20)
      - Practical/Hands-On (21-35)
      - Advanced & Best Practices (36-45)
      - Experience & Soft Skills (46-50)
    Questions:
      - Q1: "What is Shopify and how does it differ from WooCommerce?"
        A: >
          Shopify is SaaS-hosted with built-in hosting, checkout, and security.
          WooCommerce is a WordPress plugin requiring self-hosting and plugins.
      - Q2: "What is Liquid?"
        A: "Shopify’s templating language used in themes."
      - Q3: "Explain Sections & Blocks in Shopify themes."
        A: "Sections are modular theme components; Blocks are customizable elements inside sections."
      - Q4: "What is the difference between Public Apps and Custom Apps?"
        A: "Public apps are available in the App Store; Custom apps are built for a single store."
      - Q5: "Explain Shopify’s APIs."
        A: "Admin API for store data, Storefront API for headless frontends, Webhooks for events."
      - Q6: "What is Hydrogen?"
        A: "React-based framework for building custom storefronts."
      - Q7: "How does checkout work in Shopify?"
        A: "Locked for most merchants; customizable on Shopify Plus using Checkout Extensibility."
      - Q8: "What are Metafields?"
        A: "Custom fields extending Shopify objects."
      - Q9: "How does Shopify scale globally?"
        A: "SaaS model with CDN, auto-scaling, and secure checkout."
      - Q10: "What tools help developers build Shopify apps?"
        A: "Shopify CLI, Polaris, App Bridge."
      - Q11: "Explain Dawn theme."
        A: "Shopify’s reference theme for learning and customization."
      - Q12: "What are Online Store 2.0 features?"
        A: "Sections everywhere, JSON templates, app blocks."
      - Q13: "What’s the difference between Admin API REST vs GraphQL?"
        A: "GraphQL allows flexible queries; REST is simpler but less efficient."
      - Q14: "How do you register a webhook in Shopify?"
        A: "Via Admin API or CLI, specifying topic (e.g., orders/create)."
      - Q15: "What is App Bridge?"
        A: "JavaScript library for embedding Shopify apps in the Admin UI."
      - Q16: "What is Polaris?"
        A: "Shopify’s React UI library for apps."
      - Q17: "How do you add a custom field to a product?"
        A: "Use Metafields."
      - Q18: "What are Shopify Scripts?"
        A: "Custom logic for checkout (Shopify Plus only)."
      - Q19: "Explain Checkout Extensibility."
        A: "New Shopify Plus framework for customizing checkout."
      - Q20: "What is Shopify Plus?"
        A: "Enterprise version with advanced features."
      - Q21: "Write Liquid code to loop through collection products."
        A: |
          {% for product in collection.products %}
            <h2>{{ product.title }}</h2>
            <p>{{ product.price | money }}</p>
          {% endfor %}
      - Q22: "Show compare-at price and discount with Liquid."
        A: |
          {% if product.compare_at_price > product.price %}
            <span>{{ product.price | money }}</span>
            <span>{{ product.compare_at_price | money }}</span>
          {% endif %}
      - Q23: "GraphQL query to fetch products."
        A: |
          {
            products(first: 5) {
              edges {
                node {
                  title
                  handle
                }
              }
            }
          }
      - Q24: "How do you create a new Section?"
        A: "Add file under /sections, define schema JSON, reference in template."
      - Q25: "How do you display a product image in Liquid?"
        A: "{{ product.featured_image | image_url }}"
      - Q26: "How do you paginate products in Liquid?"
        A: "{% paginate collection.products by 12 %} ... {% endpaginate %}"
      - Q27: "How to fetch products with Storefront API in React?"
        A: "Use GraphQL query inside Apollo or fetch call."
      - Q28: "How to add a custom app block?"
        A: "Define app block in schema, render via Liquid."
      - Q29: "How do you test webhooks locally?"
        A: "Use ngrok or tunneling for localhost endpoint."
      - Q30: "How to secure a Shopify app?"
        A: "Use OAuth 2.0 and verify HMAC signatures."
      - Q31: "How do you filter collections in Liquid?"
        A: "{% for product in collections['summer'].products %}"
      - Q32: "How to show variant options?"
        A: "{% for variant in product.variants %} {{ variant.title }} {% endfor %}"
      - Q33: "What is the difference between theme.liquid and template.liquid?"
        A: "theme.liquid is global layout; templates are page-specific."
      - Q34: "How do you integrate third-party APIs?"
        A: "Build custom apps and call external APIs via serverless functions."
      - Q35: "How do you optimize a Shopify theme?"
        A: "Minify assets, lazy load images, use Shopify CDN."
      - Q36: "Explain best practices for Shopify SEO."
        A: "Use clean URLs, structured data, alt tags, fast loading."
      - Q37: "How to handle multi-currency?"
        A: "Use Shopify Payments or APIs with currency conversion."
      - Q38: "Explain Headless Shopify benefits."
        A: "Full control of frontend with React/Next.js."
      - Q39: "What is a sales channel in Shopify?"
        A: "External selling platforms like Facebook, Amazon integrated with Shopify."
      - Q40: "What is a storefront access token?"
        A: "Used for authenticating Storefront API queries."
      - Q41: "How do you manage environment variables in Shopify apps?"
        A: "Use dotenv or Shopify CLI config."
      - Q42: "How to implement subscription logic?"
        A: "Use Shopify Billing API or third-party apps."
      - Q43: "How do you migrate from WooCommerce to Shopify?"
        A: "Export products/customers/orders and import via Shopify."
      - Q44: "What is the Partner Dashboard?"
        A: "Platform for creating dev stores, apps, and managing clients."
      - Q45: "How to test Shopify themes?"
        A: "Preview via Shopify CLI, test with multiple products and orders."
      - Q46: "How do you explain your React experience for Shopify Hydrogen?"
        A: "Hydrogen is React-based; Next.js concepts transfer directly."
      - Q47: "How do you explain WooCommerce experience for Shopify?"
        A: "Concepts like products, checkout, APIs map to Shopify."
      - Q48: "How do you handle clients asking for custom checkout?"
        A: "Explain limitations on Standard Shopify, recommend Shopify Plus."
      - Q49: "Why would you choose GraphQL over REST?"
        A: "Efficient, reduces over-fetching, flexible queries."
      - Q50: "How do you quickly ramp up on Shopify?"
        A: "By leveraging React/Next.js and WooCommerce knowledge, focusing on Liquid, APIs, and Shopify CLI."

