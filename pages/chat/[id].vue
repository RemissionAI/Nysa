<template>
    <div class="chat-interface">
        <TopBar>
            <p>Share</p>
        </TopBar>

        <div class="messages-list">
            <div class="message">
                <h2 class="user">Is it safe to consume coffe?</h2>
                <div class="bot">
                    the safety of consuming coffee for individuals with lupus depends on various factors. While coffee
                    contains antioxidants and other beneficial compounds, it also contains caffeine, which can have
                    negative
                    effects.
                    Caffeine can stimulate the central nervous system, making us feel energized and focused. It can also
                    stimulate the respiratory and cardiovascular systems. An average eight-ounce cup of coffee contains
                    between 95-200 mg of caffeine, and decaffeinated coffee has about 3 mg. The U.S. Food and Drug
                    Administration considers it safe to consume up to 400 mg of caffeine a day.
                    However, for individuals with lupus, consuming coffee may have additional implications. Coffee can
                    cause
                    stomach upset and heartburn, increase blood pressure, and interfere with the ability to absorb
                    calcium,
                    contributing to the development of osteoporosis. Caffeine can also negatively impact sleep quality,
                    which is a concern for individuals with lupus who need to manage symptoms and flares.
                    On the other hand, some studies suggest that caffeine may increase the release of anti-inflammatory
                    proteins, suppress T-cell, B-cell, and antibody production, and decrease the prevalence of certain
                    lupus
                    manifestations. However, more research is needed to confirm these findings.
                    Therefore, it is essential for individuals with lupus to talk to their healthcare practitioner about
                    their coffee consum ption. They can discuss the potential benefits and risks and determine if coffee
                    is
                    a healthy choice for them based on their individual health situation.
                </div>
            </div>
            <div class="message">
                <h2 class="user">What is methotrexate?</h2>
                <div class="bot">
                    Methotrexate is a medication commonly used in the treatment of rheumatoid arthritis and lupus,
                    particularly for alleviating joint pain and swelling. It was approved by the FDA in the late 1980s
                    for arthritis treatment and works by interfering with the production of folic acid, a building block
                    for growing cells in the body. By hindering the growth of certain cells, including those of the
                    immune system, methotrexate is also steroid-sparing, allowing for lower doses of steroid therapy and
                    reduced side effects. The medication is typically taken as a tablet in doses of 7.5 to 25 milligrams
                    (mg) per week, but it can also be given as an injection. Improvements from methotrexate therapy can
                    be felt in 3-6 weeks, with full benefits taking up to 3 months. If a dose is missed, it can usually
                    be taken up to 4 or 5 days later, but if beyond that window, it's important to consult a doctor for
                </div>
            </div>

            <div class="message">
                <h2 class="user">Managing Lupus Disease Progression</h2>
                <div class="bot">
                    While it's important to note that there is no cure for lupus, there are several strategies that can
                    help manage the disease and potentially slow its progression. Here are some key points to consider:
                    1. Medication Adherence

                    One of the most crucial aspects of managing lupus is taking your medications as prescribed:

                    Take prednisone and other medications exactly as directed by your doctor.
                    Never discontinue or change your dosage without consulting your physician first.
                    Changing medication dosage without medical supervision can result in potentially harmful side
                    effects.

                    2. Regular Communication with Your Doctor

                    Maintaining open communication with your healthcare provider is essential:

                    Continually review your medication dosage with your doctor to ensure you're taking the lowest
                    possible dose that still effectively manages your symptoms.
                    Inform your doctor if your symptoms improve or worsen, or if there are any changes in your health
                    during treatment.
                    Your dosage may need adjusting during times of unusual stress on your body, such as surgery, dental
                    work, illness, infection, or severe asthma attacks.

                    3. Lifestyle Modifications

                    Making certain lifestyle changes can help manage lupus symptoms and potentially slow disease
                    progression:
                    Quit Smoking

                    If you smoke, commit to quitting. Studies have confirmed that smoking worsens many aspects of lupus
                    and may trigger flares.
                    Ask your doctor for help with smoking cessation if needed.

                    Manage Fatigue

                    Set your schedule to allow for adequate rest.
                    Get sufficient sleep and engage in some form of physical exercise each day.
                    Learn to listen to your body and take breaks when needed.

                    Prevent Infections

                    Reducing the risk of infections is crucial for managing lupus. Here are some strategies:

                    Maintain good hygiene habits.
                    Treat cuts and scrapes immediately.
                    Keep a clean and tidy home.
                    Stay away from people with infections.
                    Stay hydrated.
                    Eat a nutritious diet and maintain a healthy weight.
                    Monitor your body temperature regularly and report any signs of fever immediately.

                    4. Regular Health Screenings and Vaccinations

                    Complete recommended health screenings as advised by your healthcare provider.
                    Get vaccinations when advised by your trusted healthcare practitioner.

                    5. Maintain Low Disease Activity

                    Achieving and maintaining low lupus disease activity is crucial for preventing complications and
                    potentially slowing disease progression.
                    6. Take Care of Your Mental Health

                    Don't neglect your emotional well-being. Taking care of your mental health can positively impact
                    your overall health and potentially help manage lupus symptoms.

                    I hope this information helps. Remember to consult with your healthcare provider for personalized
                    medical advice.
                </div>
            </div>
        </div>

        <div class="message-input">
            <MessageInput />
        </div>
    </div>
</template>

<style lang="scss" scoped>
.chat-interface {
    max-width: 888px;
    height: 100vh;
    padding-bottom: 42px;
    margin: auto;
    display: flex;
    flex-direction: column;

    .messages-list {
        flex-grow: 1;
        overflow: auto;

        .message {
            margin: 2rem 0;

            .user {
                font-family: var(--font-family-secondary);
                margin-bottom: 10px;
            }

            .bot {
                color: var(--color-text-secondary);
                font: var(--text-md-regular);
            }

        }


    }
}
</style>