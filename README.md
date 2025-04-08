✈ Extracting Handwritten Ticket Data using UiPath and Generative AI

To automate the extraction of handwritten data from a scanned airline ticket (in this case, Biman Bangladesh Airlines), the following approach was taken using UiPath and Generative AI capabilities:
✅ Tools Used:

    UiPath Studio / Document Understanding Framework

    AI Center / Generative AI Integration

    OCR Engine (Tesseract / Google Vision OCR / Azure OCR)

    Image File (Scanned Handwritten Ticket)

🔍 Step-by-Step Breakdown:

    Document Digitization

        The handwritten airline ticket (scanned image) was input into UiPath.

        A Document Understanding Workflow was created using the IntelligentOCR and Classification/Extraction scopes.

    OCR Processing

        Integrated OCR engines (e.g., Google Vision or Azure Read API) were used to extract handwritten fields like:

            Passenger name

            Flight number

            Origin and Destination

            Fare details

            Baggage info

    Generative AI Assistance

        Post OCR, Generative AI (like OpenAI or Azure OpenAI) was integrated via UiPath's AI Center or API call to:

            Interpret ambiguous handwriting

            Normalize extracted fields (e.g., standardizing date formats, airline codes)

            Auto-correct or validate extracted flight codes, fare classes, etc.

    Structured Data Output

        The output was structured in a DataTable or JSON, ready to be:

            Sent to a database

            Used for downstream RPA tasks (e.g., form filling, system update)

            Exported as Excel or PDF for audit purposes

    Post-Processing & Human Validation (Optional)

        Validation Station in UiPath was optionally configured to allow a human reviewer to verify the data, especially for complex or unclear handwriting.

🎯 Benefits of This Approach:

    ✅ Accurate extraction from non-standard, handwritten documents

    ✅ Seamless integration of OCR + Generative AI in UiPath

    ✅ Faster processing of legacy documents

    ✅ Scalable automation for similar tickets or travel records
