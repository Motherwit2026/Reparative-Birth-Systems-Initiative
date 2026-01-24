# Reparative-Birth-Systems-Initiative
Community-Governed Knowledge &amp; Policy Infrastructure for Birth Justice Empowering Communities to Advance Equitable Maternal Health Policies
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Reparative Birth Systems Initiative | Community-Governed Knowledge & Policy Infrastructure</title>
    <link href="https://fonts.googleapis.com/css2?family=Cormorant:wght@300;400;500;600;700&family=Work+Sans:wght@300;400;500;600&display=swap" rel="stylesheet">
    <style>
        :root {
            --earth-clay: #B85C38;
            --deep-earth: #5C3317;
            --sacred-gold: #D4A574;
            --ancestral-purple: #4A2C4A;
            --life-green: #697B5B;
            --cream: #F5F1E8;
            --warm-white: #FFFBF5;
            --shadow-brown: #3D2817;
            --vibrant-coral: #FF6B6B;
            --vibrant-pink: #FF69B4;
            --vibrant-orange: #FFC371;
            --vibrant-yellow: #FFE66D;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Work Sans', sans-serif;
            color: var(--deep-earth);
            background: var(--warm-white);
            line-height: 1.7;
            overflow-x: hidden;
        }

        .hero {
            min-height: 100vh;
            background: linear-gradient(135deg, var(--ancestral-purple) 0%, var(--deep-earth) 100%);
            position: relative;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 2rem;
            overflow: hidden;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: 
                radial-gradient(circle at 20% 80%, rgba(212, 165, 116, 0.15) 0%, transparent 50%),
                radial-gradient(circle at 80% 20%, rgba(105, 123, 91, 0.15) 0%, transparent 50%);
            animation: breathe 8s ease-in-out infinite;
        }

        /* Decorative floral patterns inspired by the vibrant imagery */
        .hero::after {
            content: '';
            position: absolute;
            bottom: -100px;
            right: -100px;
            width: 600px;
            height: 600px;
            background: 
                radial-gradient(circle at 30% 30%, rgba(255, 107, 107, 0.2) 0%, transparent 40%),
                radial-gradient(circle at 70% 70%, rgba(255, 195, 113, 0.2) 0%, transparent 40%),
                radial-gradient(circle at 50% 50%, rgba(212, 165, 116, 0.15) 0%, transparent 50%);
            border-radius: 50%;
            animation: floatFloral 15s ease-in-out infinite;
        }

        @keyframes floatFloral {
            0%, 100% { transform: translate(0, 0) scale(1); }
            50% { transform: translate(-50px, -50px) scale(1.1); }
        }

        @keyframes breathe {
            0%, 100% { opacity: 0.6; }
            50% { opacity: 1; }
        }

        .hero-content {
            max-width: 1200px;
            text-align: center;
            position: relative;
            z-index: 2;
            animation: fadeInUp 1.2s ease-out;
        }

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(40px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .hero h1 {
            font-family: 'Cormorant', serif;
            font-size: clamp(2.5rem, 7vw, 5rem);
            font-weight: 400;
            color: var(--warm-white);
            margin-bottom: 1.5rem;
            letter-spacing: -0.02em;
            line-height: 1.2;
        }

        .hero h1 strong {
            font-weight: 600;
            color: var(--sacred-gold);
            display: block;
            margin-top: 0.5rem;
        }

        .hero-subtitle {
            font-size: clamp(1.1rem, 2.3vw, 1.6rem);
            color: var(--cream);
            font-weight: 300;
            margin-bottom: 2.5rem;
            animation: fadeInUp 1.2s ease-out 0.2s both;
        }

        .cta-buttons {
            display: flex;
            gap: 1.5rem;
            justify-content: center;
            flex-wrap: wrap;
            animation: fadeInUp 1.2s ease-out 0.4s both;
        }

        .btn {
            padding: 1rem 2.5rem;
            font-size: 1.1rem;
            font-weight: 500;
            text-decoration: none;
            border-radius: 0;
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
            position: relative;
            overflow: hidden;
            font-family: 'Work Sans', sans-serif;
            letter-spacing: 0.05em;
            text-transform: uppercase;
            font-size: 0.95rem;
        }

        .btn-primary {
            background: var(--sacred-gold);
            color: var(--deep-earth);
            border: 2px solid var(--sacred-gold);
        }

        .btn-primary::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: var(--earth-clay);
            transition: left 0.4s ease;
            z-index: -1;
        }

        .btn-primary:hover::before {
            left: 0;
        }

        .btn-primary:hover {
            color: var(--warm-white);
            border-color: var(--earth-clay);
        }

        .btn-secondary {
            background: transparent;
            color: var(--cream);
            border: 2px solid var(--cream);
        }

        .btn-secondary:hover {
            background: var(--cream);
            color: var(--ancestral-purple);
        }

        section {
            padding: 6rem 2rem;
            max-width: 1400px;
            margin: 0 auto;
        }

        .section-title {
            font-family: 'Cormorant', serif;
            font-size: clamp(2.5rem, 5vw, 4rem);
            font-weight: 500;
            color: var(--deep-earth);
            margin-bottom: 1rem;
            position: relative;
            display: inline-block;
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 0;
            width: 60%;
            height: 3px;
            background: linear-gradient(90deg, var(--vibrant-coral), var(--vibrant-orange), var(--sacred-gold));
        }

        .section-title::before {
            content: '✿';
            position: absolute;
            left: -50px;
            top: 50%;
            transform: translateY(-50%);
            font-size: 2rem;
            color: var(--vibrant-pink);
            opacity: 0.3;
        }

        .section-subtitle {
            font-size: 1.3rem;
            color: var(--life-green);
            margin-bottom: 3rem;
            font-style: italic;
        }

        .problem-section {
            background: var(--cream);
        }

        .problem-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2.5rem;
            margin-top: 3rem;
        }

        .problem-card {
            background: var(--warm-white);
            padding: 2.5rem;
            border-left: 4px solid var(--vibrant-coral);
            transition: all 0.3s ease;
            position: relative;
        }

        .problem-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 4px;
            height: 0;
            background: linear-gradient(180deg, var(--vibrant-pink), var(--vibrant-yellow));
            transition: height 0.3s ease;
        }

        .problem-card:hover::before {
            height: 100%;
        }

        .problem-card:hover {
            transform: translateX(10px);
            box-shadow: -15px 15px 30px rgba(0, 0, 0, 0.1);
        }

        .problem-card h3 {
            font-family: 'Cormorant', serif;
            font-size: 1.8rem;
            color: var(--deep-earth);
            margin-bottom: 1rem;
        }

        .shift-section {
            background: linear-gradient(135deg, var(--ancestral-purple) 0%, var(--shadow-brown) 100%);
            color: var(--cream);
            position: relative;
            overflow: hidden;
        }

        .shift-section::before {
            content: '';
            position: absolute;
            top: -50%;
            right: -20%;
            width: 800px;
            height: 800px;
            background: 
                radial-gradient(circle at 30% 30%, rgba(255, 107, 107, 0.15) 0%, transparent 50%),
                radial-gradient(circle at 60% 60%, rgba(255, 195, 113, 0.15) 0%, transparent 50%),
                radial-gradient(circle at 50% 50%, rgba(212, 165, 116, 0.1) 0%, transparent 70%);
            animation: float 20s ease-in-out infinite;
        }

        .shift-section::after {
            content: '❀';
            position: absolute;
            bottom: 10%;
            left: 5%;
            font-size: 15rem;
            color: var(--vibrant-coral);
            opacity: 0.05;
            animation: floatFloral 12s ease-in-out infinite;
        }

        @keyframes float {
            0%, 100% { transform: translate(0, 0) rotate(0deg); }
            50% { transform: translate(-30px, 30px) rotate(10deg); }
        }

        .shift-section .section-title {
            color: var(--sacred-gold);
        }

        .shift-section .section-subtitle {
            color: var(--cream);
        }

        .flow-comparison {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 3rem;
            margin-top: 3rem;
            position: relative;
            z-index: 2;
        }

        .flow-box {
            background: rgba(245, 241, 232, 0.05);
            padding: 3rem;
            border: 2px solid rgba(212, 165, 116, 0.3);
            backdrop-filter: blur(10px);
            transition: all 0.4s ease;
        }

        .flow-box:hover {
            background: rgba(245, 241, 232, 0.1);
            border-color: var(--sacred-gold);
            transform: scale(1.03);
        }

        .flow-box h3 {
            font-family: 'Cormorant', serif;
            font-size: 2rem;
            color: var(--sacred-gold);
            margin-bottom: 1.5rem;
        }

        .flow-box .flow-label {
            font-size: 0.9rem;
            text-transform: uppercase;
            letter-spacing: 0.1em;
            color: var(--earth-clay);
            margin-bottom: 1rem;
        }

        .flow-arrow {
            font-size: 2rem;
            color: var(--sacred-gold);
            margin: 1rem 0;
        }

        .components-section {
            background: var(--warm-white);
        }

        .component-boxes {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(450px, 1fr));
            gap: 3rem;
            margin-top: 3rem;
        }

        .component-box {
            background: var(--cream);
            padding: 3rem;
            border-left: 5px solid var(--vibrant-coral);
            position: relative;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .component-box::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 5px;
            height: 0;
            background: linear-gradient(180deg, var(--vibrant-pink), var(--vibrant-orange));
            transition: height 0.4s ease;
        }

        .component-box:hover::before {
            height: 100%;
        }

        .component-box:hover {
            transform: translateX(10px);
            box-shadow: -20px 20px 40px rgba(0, 0, 0, 0.1);
        }

        .component-box h3 {
            font-family: 'Cormorant', serif;
            font-size: 2.2rem;
            color: var(--deep-earth);
            margin-bottom: 0.5rem;
        }

        .component-box .subtitle {
            font-size: 1.1rem;
            color: var(--earth-clay);
            margin-bottom: 1.5rem;
            font-weight: 500;
        }

        .component-icon {
            font-size: 3rem;
            margin-bottom: 1rem;
            background: linear-gradient(135deg, var(--vibrant-coral), var(--vibrant-orange));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .component-features {
            margin-top: 2rem;
            padding-top: 2rem;
            border-top: 1px solid rgba(92, 51, 23, 0.2);
        }

        .component-features h4 {
            font-family: 'Cormorant', serif;
            font-size: 1.4rem;
            margin-bottom: 1rem;
            color: var(--deep-earth);
        }

        .component-features ul {
            margin-left: 1.5rem;
            line-height: 2;
        }

        .principles-section {
            background: var(--cream);
        }

        .principles-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 2rem;
            margin-top: 3rem;
        }

        .principle-card {
            background: var(--warm-white);
            padding: 2.5rem;
            position: relative;
            transition: all 0.4s ease;
        }

        .principle-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: linear-gradient(90deg, var(--vibrant-coral), var(--vibrant-orange), var(--vibrant-yellow));
        }

        .principle-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.15);
        }

        .principle-card h3 {
            font-family: 'Cormorant', serif;
            font-size: 1.8rem;
            color: var(--deep-earth);
            margin-bottom: 1rem;
        }

        .quote-block {
            font-family: 'Cormorant', serif;
            font-size: 1.8rem;
            font-style: italic;
            color: var(--ancestral-purple);
            text-align: center;
            padding: 3rem 2rem;
            margin: 4rem 0;
            position: relative;
            max-width: 900px;
            margin-left: auto;
            margin-right: auto;
        }

        .quote-block::before {
            content: '"';
            font-size: 8rem;
            color: var(--sacred-gold);
            opacity: 0.2;
            position: absolute;
            top: -2rem;
            left: 0;
            font-family: 'Cormorant', serif;
        }

        .contact {
            background: var(--warm-white);
            text-align: center;
        }

        .contact-content {
            max-width: 800px;
            margin: 0 auto;
        }

        .contact-info {
            margin-top: 3rem;
            display: flex;
            flex-direction: column;
            gap: 1.5rem;
        }

        .contact-item {
            font-size: 1.2rem;
            color: var(--deep-earth);
        }

        .contact-item a {
            color: var(--earth-clay);
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s ease;
        }

        .contact-item a:hover {
            color: var(--sacred-gold);
        }

        footer {
            background: var(--deep-earth);
            color: var(--cream);
            padding: 3rem 2rem;
            text-align: center;
        }

        footer p {
            margin-bottom: 0.5rem;
        }

        @media (max-width: 768px) {
            .hero {
                min-height: 80vh;
            }

            section {
                padding: 4rem 1.5rem;
            }

            .component-boxes,
            .flow-comparison {
                grid-template-columns: 1fr;
            }

            .component-box {
                padding: 2rem;
            }

            .cta-buttons {
                flex-direction: column;
                align-items: center;
            }

            .btn {
                width: 100%;
                max-width: 300px;
            }
        }

        .fiscal-section {
            background: var(--cream);
        }

        .fiscal-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2.5rem;
            margin-top: 3rem;
        }

        .fiscal-card {
            background: var(--warm-white);
            padding: 2.5rem;
            border-left: 4px solid var(--life-green);
        }

        .fiscal-card h3 {
            font-family: 'Cormorant', serif;
            font-size: 1.8rem;
            color: var(--deep-earth);
            margin-bottom: 1rem;
        }

        /* Decorative floral accents */
        .decorative-flower {
            position: absolute;
            opacity: 0.08;
            color: var(--vibrant-coral);
            font-size: 8rem;
            pointer-events: none;
            animation: floatFloral 15s ease-in-out infinite;
        }

        .problem-section {
            position: relative;
        }

        .problem-section::before {
            content: '❀';
            position: absolute;
            top: 5%;
            right: 5%;
            font-size: 12rem;
            color: var(--vibrant-pink);
            opacity: 0.05;
            animation: floatFloral 18s ease-in-out infinite;
        }

        .components-section {
            position: relative;
        }

        .components-section::after {
            content: '✿';
            position: absolute;
            bottom: 10%;
            right: 8%;
            font-size: 10rem;
            color: var(--vibrant-orange);
            opacity: 0.06;
            animation: floatFloral 20s ease-in-out infinite;
        }

        .contact {
            position: relative;
        }

        .contact::before {
            content: '❁';
            position: absolute;
            top: 10%;
            left: 5%;
            font-size: 10rem;
            color: var(--vibrant-coral);
            opacity: 0.05;
            animation: floatFloral 16s ease-in-out infinite;
        }
    </style>
</head>
<body>
    <div class="hero">
        <div class="hero-content">
            <h1>
                Reparative Birth Systems Initiative
                <strong>Community-Governed Knowledge & Policy Infrastructure for Birth Justice</strong>
            </h1>
            <p class="hero-subtitle">
                Empowering Communities to Advance Equitable Maternal Health Policies
            </p>
            <div class="cta-buttons">
                <a href="#framework" class="btn btn-primary">Explore the Framework</a>
                <a href="#contact" class="btn btn-secondary">Partnership Opportunities</a>
            </div>
        </div>
    </div>

    <section id="crisis" class="problem-section">
        <h2 class="section-title">The Maternal Health & Knowledge Crisis</h2>
        <p class="section-subtitle">Understanding the Need for Systems Change</p>

        <div class="problem-grid">
            <div class="problem-card">
                <h3>Disproportionate Maternal Mortality Among Black Women</h3>
                <p>Black women experience significantly higher maternal mortality rates than other groups, highlighting urgent health disparities driven by systemic healthcare inequities and social determinants of health. Addressing these disparities requires systemic change to achieve equitable birth justice.</p>
            </div>

            <div class="problem-card">
                <h3>Disempowerment in Defining Evidence</h3>
                <p>Impacted communities have restricted roles in shaping what counts as valid maternal health evidence. Excluding lived experiences creates significant gaps in understanding maternal health disparities, resulting in inadequate responses that fail to address real community needs.</p>
            </div>

            <div class="problem-card">
                <h3>Limitations of Academic Research</h3>
                <p>Current research models omit valuable insights from community members, with centralized institutional control limiting diverse perspectives. Overreliance on quantitative data restricts fuller understanding of complex maternal health issues, while published harm often goes unaccountable.</p>
            </div>
        </div>

        <div class="quote-block">
            Traditional maternal health research extracts data from BIPOC communities without community control over findings or applications. Evidence-based policy rarely incorporates community-defined health indicators or cultural practices.
        </div>
    </section>

    <section id="shift" class="shift-section">
        <h2 class="section-title">Inverting the Knowledge Hierarchy</h2>
        <p class="section-subtitle">A Revolutionary Paradigm Shift</p>

        <div class="flow-comparison">
            <div class="flow-box">
                <div class="flow-label">Traditional Approach</div>
                <h3>Top-Down Knowledge Flow</h3>
                <div class="flow-arrow">↓</div>
                <p style="font-size: 1.1rem; line-height: 1.8;">
                    <strong>Academia</strong><br>
                    generates research and evidence
                </p>
                <div class="flow-arrow">↓</div>
                <p style="font-size: 1.1rem; line-height: 1.8;">
                    <strong>Community</strong><br>
                    becomes research subjects
                </p>
                <div class="flow-arrow">↓</div>
                <p style="font-size: 1.1rem; line-height: 1.8;">
                    <strong>Policy</strong><br>
                    developed externally, limiting community agency
                </p>
            </div>

            <div class="flow-box">
                <div class="flow-label">RBSI Model</div>
                <h3>Community-Centered Flow</h3>
                <div class="flow-arrow">↓</div>
                <p style="font-size: 1.1rem; line-height: 1.8;">
                    <strong>Community</strong><br>
                    generates knowledge and defines evidence
                </p>
                <div class="flow-arrow">↓</div>
                <p style="font-size: 1.1rem; line-height: 1.8;">
                    <strong>Evidence</strong><br>
                    community insights inform robust evidence creation
                </p>
                <div class="flow-arrow">↓</div>
                <p style="font-size: 1.1rem; line-height: 1.8;">
                    <strong>Policy</strong><br>
                    driven by community-controlled evidence
                </p>
                <p style="margin-top: 2rem; font-style: italic; color: var(--sacred-gold);">
                    Academia participates as invited collaborators, maintaining accountability to community leadership
                </p>
            </div>
        </div>
    </section>

    <section id="framework">
        <h2 class="section-title">RBSI Framework</h2>
        <p class="section-subtitle">Building a Community-Governed Ecosystem</p>

        <div style="background: linear-gradient(135deg, var(--vibrant-coral) 0%, var(--vibrant-orange) 50%, var(--vibrant-yellow) 100%); padding: 0.5rem; margin: 3rem auto; max-width: 800px; position: relative;">
            <div style="background: var(--warm-white); padding: 3rem; text-align: center;">
                <p style="font-family: 'Cormorant', serif; font-size: 1.8rem; font-style: italic; color: var(--deep-earth); line-height: 1.6;">
                    "Celebrating the beauty, strength, and wisdom of Black motherhood—<br>
                    centering lived experiences as the foundation for birth justice"
                </p>
            </div>
        </div>

        <div class="principles-grid">
            <div class="principle-card">
                <h3>Community-Generated Evidence</h3>
                <p>Communities generate evidence based on their unique experiences and priorities. RBSI supports translating community knowledge into actionable policy measures for real-world impact.</p>
            </div>

            <div class="principle-card">
                <h3>Knowledge Sovereignty</h3>
                <p>Community control ensures knowledge creation is led and governed by the community itself. Data stewardship involves responsible management aligned with community values, with ethical use and transparency promoting cultural relevance.</p>
            </div>

            <div class="principle-card">
                <h3>Leadership Development</h3>
                <p>RBSI focuses on equipping community leaders with skills for effective governance and sustained impact, maintaining stable governance systems that uphold community values and support birth justice over time.</p>
            </div>
        </div>
    </section>

    <section id="components" class="components-section">
        <h2 class="section-title">Key Components</h2>
        <p class="section-subtitle">A Dual-Program Approach</p>

        <div class="component-boxes">
            <div class="component-box">
                <div class="component-icon">◈</div>
                <h3>Reparative Birth Evidence Network</h3>
                <p class="subtitle">RBEN</p>
                <p style="font-size: 1.1rem; margin-bottom: 1.5rem;">
                    Reimagining what counts as evidence in birth and reproductive health through a reproductive justice lens. Communities are the primary knowledge holders and interpreters of their own birth and reproductive experiences.
                </p>

                <div class="component-features">
                    <h4>Core Elements</h4>
                    <ul>
                        <li><strong>Training Community Data Stewards:</strong> Empowering community members to effectively gather, organize, and manage data that reflects lived experiences accurately</li>
                        <li><strong>Sacred Story Circles:</strong> Culturally grounded methodology to gather community insights and document determinants of birth outcomes</li>
                        <li><strong>Community-Owned Evidence:</strong> Evidence generated and owned by the community, designed to inform and support policy advocacy for meaningful change</li>
                    </ul>
                </div>
            </div>

            <div class="component-box">
                <div class="component-icon">★</div>
                <h3>Virginia Birth Justice Policy & Legislative Fellowship</h3>
                <p class="subtitle">Community-Rooted Policy Leadership</p>
                <p style="font-size: 1.1rem; margin-bottom: 1.5rem;">
                    Policy advocacy must be led by those most impacted, using evidence generated by and for their own communities. This non-extractive approach is distinct from traditional internships and academic pipelines.
                </p>

                <div class="component-features">
                    <h4>Fellowship Functions</h4>
                    <ul>
                        <li><strong>Developing Community-Rooted Policy Leaders:</strong> Building skills and confidence for community members to lead effectively in policymaking with authentic engagement</li>
                        <li><strong>Translating Evidence Into Policy:</strong> Using proprietary methods to convert community evidence into effective policy recommendations and advocacy</li>
                        <li><strong>Legislative Navigation:</strong> Identifying key stakeholders and influence pathways to strategically advance advocacy goals</li>
                        <li><strong>Ethical Advocacy:</strong> Consent-based advocacy alongside paid leadership roles creating a supportive and engaged community</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <section id="future-research" style="background: linear-gradient(135deg, rgba(255, 107, 107, 0.08), rgba(255, 195, 113, 0.08)); position: relative;">
        <h2 class="section-title">Future Community-Owned Research</h2>
        <p class="section-subtitle">Expanding the Reparative Birth Evidence Network</p>

        <div style="background: var(--warm-white); padding: 3rem; border-left: 5px solid var(--vibrant-coral); margin-bottom: 3rem;">
            <h3 style="font-family: 'Cormorant', serif; font-size: 2.5rem; color: var(--deep-earth); margin-bottom: 1rem;">
                Charlottesville Maternal Housing Instability Community Assessment
            </h3>
            <p style="font-size: 1.1rem; color: var(--earth-clay); font-weight: 500; margin-bottom: 1.5rem;">
                A Reparative Birth Evidence Network Study
            </p>
            <p style="font-size: 1.1rem; line-height: 1.8; margin-bottom: 1rem;">
                This groundbreaking 18-month community assessment documents how Charlottesville's 25-year housing crisis—rooted in historic Black displacement through urban renewal and intensified by gentrification—creates a predictable and preventable risk environment for pregnant and postpartum people, especially Black women.
            </p>
            <p style="font-size: 1.1rem; line-height: 1.8;">
                Using the RBEN framework, this study positions pregnant and postpartum people who have experienced housing instability as primary knowledge producers rather than research subjects. The Survivor Advisory Circle owns all data, leads all analysis, and controls all dissemination.
            </p>
        </div>

        <div class="problem-grid">
            <div class="problem-card">
                <h3>The 9-Domino Effect Framework</h3>
                <p>The study documents the complete sequence from generational housing displacement through pregnancy-work conflicts to birth harm and intergenerational continuation—demonstrating that housing instability during pregnancy is not merely an economic stressor but a documented contributor to adverse birth outcomes that falls disproportionately on Black women.</p>
            </div>

            <div class="problem-card">
                <h3>Community Knowledge Sovereignty</h3>
                <p>Survivor Advisory Circle (8-12 pregnant/postpartum people who experienced housing instability) has final decision-making power over research questions, data collection, analysis, dissemination, and all partnerships. Community members are the primary knowledge producers, not research subjects.</p>
            </div>

            <div class="problem-card">
                <h3>Revolutionary Research Design</h3>
                <p>Employs Sacred Story Circles, in-depth interviews, community photovoice, and birth outcomes analysis—all led by those most impacted. This is not research ON communities. This is knowledge BY communities. This is power building through truth-telling.</p>
            </div>
        </div>

        <div style="margin-top: 4rem; background: var(--cream); padding: 3rem; max-width: 900px; margin-left: auto; margin-right: auto;">
            <h3 style="font-family: 'Cormorant', serif; font-size: 2rem; margin-bottom: 1.5rem; color: var(--deep-earth);">Study Overview</h3>
            <div style="display: grid; gap: 1.5rem;">
                <div style="display: grid; grid-template-columns: 200px 1fr; gap: 1rem; align-items: start;">
                    <strong>Framework Author:</strong>
                    <span>Lisa N. Brown, Reparative Birth Systems Initiative</span>
                </div>
                <div style="display: grid; grid-template-columns: 200px 1fr; gap: 1rem; align-items: start;">
                    <strong>Study Timeline:</strong>
                    <span>18 Months</span>
                </div>
                <div style="display: grid; grid-template-columns: 200px 1fr; gap: 1rem; align-items: start;">
                    <strong>Target Budget:</strong>
                    <span>$385,000</span>
                </div>
                <div style="display: grid; grid-template-columns: 200px 1fr; gap: 1rem; align-items: start;">
                    <strong>Location:</strong>
                    <span>Charlottesville/Albemarle County, Virginia</span>
                </div>
                <div style="display: grid; grid-template-columns: 200px 1fr; gap: 1rem; align-items: start;">
                    <strong>Core Methods:</strong>
                    <span>Sacred Story Circles, In-Depth Interviews, Community Photovoice, Provider Stakeholder Interviews, Quantitative Survey, Birth Outcomes Analysis</span>
                </div>
            </div>
        </div>

        <div style="margin-top: 3rem;">
            <h3 style="font-family: 'Cormorant', serif; font-size: 2rem; margin-bottom: 2rem; color: var(--deep-earth); text-align: center;">Key Research Principles</h3>
            <div class="principles-grid">
                <div class="principle-card">
                    <h3>Community-Defined Quality</h3>
                    <p>Participants feel heard and valued. Findings ring true to lived experience. Study builds community power. Evidence drives community-determined solutions. No harm caused by participation.</p>
                </div>

                <div class="principle-card">
                    <h3>Data Sovereignty</h3>
                    <p>Survivor Advisory Circle owns all data—legal, material, and intellectual ownership. Partners access data only with explicit Circle approval for specific, limited purposes. Circle can revoke access immediately if agreement violated.</p>
                </div>

                <div class="principle-card">
                    <h3>Reparation Not Extraction</h3>
                    <p>Fair compensation for expertise. Evidence supports community-determined solutions. Builds community capacity for ongoing knowledge production. Challenges systems that caused the crisis. Contributes to intergenerational healing through truth-telling.</p>
                </div>

                <div class="principle-card">
                    <h3>Liberation-Centered Analysis</h3>
                    <p>We examine systemic failures and community resistance, not individual shortcomings. Did we challenge systems or reinforce them? Did we build survivor power or extract their stories? Did we center community solutions or academic theories?</p>
                </div>
            </div>
        </div>

        <div style="margin-top: 4rem; background: linear-gradient(135deg, var(--vibrant-coral) 0%, var(--vibrant-orange) 100%); padding: 0.5rem; max-width: 900px; margin-left: auto; margin-right: auto;">
            <div style="background: var(--warm-white); padding: 3rem; text-align: center;">
                <p style="font-family: 'Cormorant', serif; font-size: 1.8rem; font-style: italic; color: var(--deep-earth); line-height: 1.6; margin-bottom: 1.5rem;">
                    "This is not research ON communities. This is knowledge BY communities. This is power building through truth-telling. This is reparation through community sovereignty."
                </p>
                <p style="font-size: 1.1rem; color: var(--life-green);">
                    — Charlottesville Maternal Housing Instability Community Assessment Framework
                </p>
            </div>
        </div>

        <div style="margin-top: 3rem; text-align: center;">
            <p style="font-size: 1.2rem; margin-bottom: 1.5rem; color: var(--deep-earth);">
                This study establishes Charlottesville as a national model for community-controlled research on housing and maternal health, creating an irrefutable case for systems change while building infrastructure for ongoing community knowledge sovereignty.
            </p>
        </div>

        <div style="margin-top: 4rem; background: var(--cream); padding: 3rem; border-left: 5px solid var(--vibrant-orange);">
            <h3 style="font-family: 'Cormorant', serif; font-size: 2.2rem; color: var(--deep-earth); margin-bottom: 1.5rem;">
                Potential Pilot Program: Maternal Housing Sanctuary
            </h3>
            <p style="font-size: 1.1rem; color: var(--earth-clay); font-weight: 500; margin-bottom: 1.5rem;">
                A Community-Controlled Initiative Following the Research
            </p>
            <p style="font-size: 1.1rem; line-height: 1.8; margin-bottom: 1rem;">
                Following the community assessment, the Maternal Housing Sanctuary Pilot Program would establish Charlottesville as Virginia's first community where pregnant and postpartum people are protected from housing displacement during the critical perinatal period.
            </p>
            <p style="font-size: 1.1rem; line-height: 1.8; margin-bottom: 1.5rem;">
                Grounded in evidence that housing instability during pregnancy increases risk of preterm birth by 73%, NICU admission by 64%, and low birth weight by similar margins, this pilot would create a replicable model for birth equity through housing justice.
            </p>

            <div style="background: var(--warm-white); padding: 2rem; margin-top: 2rem;">
                <h4 style="font-family: 'Cormorant', serif; font-size: 1.6rem; margin-bottom: 1rem; color: var(--deep-earth);">Core Program Components</h4>
                <ul style="line-height: 2; margin-left: 1.5rem;">
                    <li><strong>Protected Class Status:</strong> Establish pregnant and postpartum people (through 12 months) as protected class for housing stability interventions</li>
                    <li><strong>Mandatory Eviction Diversion:</strong> Landlords must complete diversion process before filing eviction against pregnant/postpartum tenant</li>
                    <li><strong>Emergency Rental Assistance:</strong> Up to $7,000 per household covering arrears and forward rent during maternity period</li>
                    <li><strong>Birth-Centered Housing Navigation:</strong> Community health workers with doula training embedded in prenatal care settings</li>
                    <li><strong>Legal Support:</strong> Free representation in eviction proceedings for pregnant/postpartum tenants</li>
                    <li><strong>Landlord Partnership Program:</strong> Incentives and support for housing providers maintaining stable housing for maternal households</li>
                </ul>
            </div>

            <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 2rem; margin-top: 2rem;">
                <div>
                    <p style="font-size: 2.5rem; font-family: 'Cormorant', serif; color: var(--vibrant-coral); font-weight: 600; margin-bottom: 0.5rem;">24</p>
                    <p style="font-size: 0.9rem; text-transform: uppercase; letter-spacing: 0.1em; color: var(--life-green);">Month Pilot</p>
                </div>
                <div>
                    <p style="font-size: 2.5rem; font-family: 'Cormorant', serif; color: var(--vibrant-coral); font-weight: 600; margin-bottom: 0.5rem;">150-200</p>
                    <p style="font-size: 0.9rem; text-transform: uppercase; letter-spacing: 0.1em; color: var(--life-green);">Households Protected Annually</p>
                </div>
                <div>
                    <p style="font-size: 2.5rem; font-family: 'Cormorant', serif; color: var(--vibrant-coral); font-weight: 600; margin-bottom: 0.5rem;">$2.4M</p>
                    <p style="font-size: 0.9rem; text-transform: uppercase; letter-spacing: 0.1em; color: var(--life-green);">3-Year Budget</p>
                </div>
            </div>

            <div style="margin-top: 2rem; padding: 2rem; background: linear-gradient(135deg, rgba(255, 107, 107, 0.1), rgba(255, 195, 113, 0.1));">
                <p style="font-size: 1.1rem; font-style: italic; color: var(--deep-earth); line-height: 1.8;">
                    This program represents a fundamental reframing: housing stability during pregnancy and postpartum is not a luxury or individual responsibility—it is a birth equity imperative with direct, measurable impacts on maternal and infant health.
                </p>
            </div>

            <div style="margin-top: 2rem;">
                <h4 style="font-family: 'Cormorant', serif; font-size: 1.6rem; margin-bottom: 1rem; color: var(--deep-earth);">Community Knowledge Sovereignty in Program Design</h4>
                <p style="font-size: 1.05rem; line-height: 1.8; margin-bottom: 1rem;">
                    The pilot program would continue RBEN principles through quarterly Sacred Story Circles, community data stewardship, and the Community Research Cooperative governing all program decisions. Those most impacted by the intersection of housing crisis and pregnancy would lead solution design, implementation, and evaluation.
                </p>
                <p style="font-size: 1.05rem; line-height: 1.8;">
                    Charlottesville would become Virginia's first Maternal Sanctuary City—a model of what birth equity looks like when we address the root causes of maternal health disparities, with findings providing the evidence base to transform policy across Virginia and beyond.
                </p>
            </div>
        </div>
    </section>

    <section id="fiscal" class="fiscal-section">
        <h2 class="section-title">Why Fiscal Sponsorship Matters</h2>
        <p class="section-subtitle">Infrastructure for Community Governance</p>

        <div class="fiscal-grid">
            <div class="fiscal-card">
                <h3>Legal Infrastructure & Compliance</h3>
                <p>Fiscal sponsorship delivers vital legal structure, helping projects stay compliant and protected from risks that could harm sustainability.</p>
            </div>

            <div class="fiscal-card">
                <h3>Administrative Support</h3>
                <p>Sponsors manage complex financial and regulatory tasks, providing an administrative buffer for projects to focus on their mission.</p>
            </div>

            <div class="fiscal-card">
                <h3>Community Governance</h3>
                <p>While sponsors support advocacy and compliance, the community keeps control over project direction and content.</p>
            </div>
        </div>

        <div style="margin-top: 4rem; max-width: 900px; margin-left: auto; margin-right: auto;">
            <h3 style="font-family: 'Cormorant', serif; font-size: 2rem; margin-bottom: 1.5rem; color: var(--deep-earth);">Expected Outcomes</h3>
            <div class="problem-grid" style="margin-top: 2rem;">
                <div class="problem-card">
                    <h3 style="font-size: 1.5rem;">Actionable Policy Briefs</h3>
                    <p>Concise, policy-ready briefs that empower decision-makers with clear, implementable recommendations.</p>
                </div>
                <div class="problem-card">
                    <h3 style="font-size: 1.5rem;">Emerging Policy Leaders</h3>
                    <p>A cohort of trained community policy leaders driving meaningful changes in maternal health and advocacy.</p>
                </div>
                <div class="problem-card">
                    <h3 style="font-size: 1.5rem;">Model for National Adoption</h3>
                    <p>Virginia's strengthened maternal health advocacy becomes a replicable model, amplifying best practices across communities nationwide.</p>
                </div>
            </div>
        </div>
    </section>

    <section id="principles" class="principles-section">
        <h2 class="section-title">Safeguarding Core Elements</h2>
        <p class="section-subtitle">Protecting Innovation & Community Authority</p>

        <div class="principles-grid">
            <div class="principle-card">
                <h3>Protected Training Curriculum</h3>
                <p>The training curriculum is safeguarded to preserve expertise and maintain high standards within the organization.</p>
            </div>

            <div class="principle-card">
                <h3>Ethical Policy Alignment</h3>
                <p>Policy strategies designed to ensure all practices align with ethical guidelines and organizational values.</p>
            </div>

            <div class="principle-card">
                <h3>Knowledge Transfer Protocols</h3>
                <p>Evidence translation protocols ensure valuable knowledge is transferred responsibly and securely.</p>
            </div>

            <div class="principle-card">
                <h3>Community Governance</h3>
                <p>Empowering collective decision-making while promoting transparency without risking sensitive information.</p>
            </div>
        </div>

        <div class="quote-block">
            Policies created without community involvement may unintentionally cause harm. Community-governed policies build fairness and trust, leading to sustainable, equitable solutions that better serve everyone involved.
        </div>
    </section>

    <section id="contact" class="contact">
        <div class="contact-content">
            <h2 class="section-title">Partnership Opportunities</h2>
            <p class="section-subtitle">Building Community-Governed Justice Together</p>
            
            <p style="font-size: 1.2rem; margin-bottom: 2rem; max-width: 700px; margin-left: auto; margin-right: auto;">
                We welcome fiscal sponsors, funders, academic institutions, healthcare systems, and policy organizations committed to authentic community sovereignty and birth justice.
            </p>

            <div style="background: var(--cream); padding: 2.5rem; margin-top: 3rem; max-width: 700px; margin-left: auto; margin-right: auto;">
                <h3 style="font-family: 'Cormorant', serif; font-size: 1.8rem; margin-bottom: 1.5rem; color: var(--deep-earth);">Project Information</h3>
                <p style="margin-bottom: 1rem;"><strong>Project Timeline:</strong> 36 Months</p>
                <p style="margin-bottom: 1rem;"><strong>Target Budget:</strong> $575,000</p>
                <p style="margin-bottom: 1rem;"><strong>Geographic Focus:</strong> Virginia (with replication potential)</p>
                <p style="margin-top: 1.5rem;"><strong>Fiscal Sponsor:</strong> Elephant Circle (MOU 1/26/2026)</p>
            </div>

            <div class="contact-info">
                <div class="contact-item">
                    <strong>Project Director</strong><br>
                    Lisa N. Brown
                </div>
                <div class="contact-item">
                    <strong>Organization</strong><br>
                    Motherwit Akoma Services, LLC dba Motherwit Birth Services
                </div>
                <div class="contact-item">
                    <strong>Email:</strong> <a href="/cdn-cgi/l/email-protection#7f13160c1e3f12100b171a0d08160b1d160d0b170c1a0d09161c1a0c511c1012"><span class="__cf_email__" data-cfemail="610d081200210c0e15090413160815030813150912041317080204124f020e0c">[email&#160;protected]</span></a>
                </div>
                <div class="contact-item">
                    <strong>Phone:</strong> <a href="tel:434-466-8849">434-466-8849</a>
                </div>
            </div>

            <div style="margin-top: 3rem; padding: 2rem; background: var(--warm-white); max-width: 700px; margin-left: auto; margin-right: auto;">
                <p style="font-size: 0.95rem; color: var(--shadow-brown);">
                    <strong>Confidentiality Notice:</strong> This initiative contains proprietary and confidential information about innovative community participatory research methodologies and policy advocacy frameworks. Partnership discussions require signed Non-Disclosure Agreements and formal partnership proposals demonstrating commitment to community ownership and control.
                </p>
            </div>

            <div style="margin-top: 2rem; padding: 2rem; background: linear-gradient(135deg, rgba(255, 107, 107, 0.1), rgba(255, 195, 113, 0.1)); max-width: 700px; margin-left: auto; margin-right: auto; border-left: 4px solid var(--vibrant-coral);">
                <p style="font-size: 1rem; color: var(--deep-earth); line-height: 1.8;">
                    <strong>Visual Identity:</strong> RBSI honors and centers the beauty of Black motherhood through vibrant, culturally-grounded visual storytelling. Our communications celebrate the strength, wisdom, and sacred nature of birth experiences in Black communities.
                </p>
            </div>
        </div>
    </section>

    <footer>
        <p style="font-family: 'Cormorant', serif; font-size: 1.5rem; margin-bottom: 1rem;">
            Reparative Birth Systems Initiative
        </p>
        <p>Community-Governed Knowledge & Policy Infrastructure for Birth Justice</p>
        <p style="margin
