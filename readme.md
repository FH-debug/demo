flowchart TD
    START([🧪 Start Experiment 3]) --> SETUP

    subgraph SETUP ["⚙️ Setup"]
        SETUP[Collect ~50 mL of 0.00200 M KSCN\nHalf-fill burette a] --> BURETTES
        BURETTES[Prepare burettes:\nb = 0.00200 M Fe NO3 3\nc = Distilled Water]
    end

    BURETTES --> PARTA

    subgraph PARTA ["📊 Part A: Calibration Curve"]
        A1[Collect ~175 mL of\n0.200 M Fe NO3 3] --> A2
        A2[Prepare 3 x 50 mL volumetric flasks\nRinse with distilled water,\nthen with Fe NO3 3 solution] --> A3
        A3[From burette a, deliver KSCN:\nFlask 1 → 1.0 mL\nFlask 2 → 2.0 mL\nFlask 3 → 3.0 mL] --> A4
        A4[Fill all flasks to 50.00 mL mark\nwith 0.200 M Fe NO3 3] --> A5
        A5[Invert each flask several times\nDO NOT SHAKE] --> A6
        A6[Standardize spectrophotometer\nwith DI water blank at 447 nm] --> A7
        A7[Rinse cuvette 3x with each solution\nFill 3/4 full, wipe outside with Kimwipe] --> A8
        A8[Measure absorbance A\nfor each of the 3 flasks\nRecord values] --> A9
        A9[Rinse cuvettes with DI water]
    end

    A9 --> PARTB

    subgraph PARTB ["⚗️ Part B: Equilibrium Constant"]
        B1[Label 3 clean dry test tubes 1–3] --> B2
        B2[From burette a, add 0.00200 M KSCN:\nTube 1 → 2.00 mL\nTube 2 → 3.00 mL\nTube 3 → 4.00 mL] --> B3
        B3[From burette b, add 0.00200 M Fe NO3 3:\nAll tubes → 5.00 mL] --> B4
        B4[From burette c, add DI water:\nTube 1 → 3.00 mL\nTube 2 → 2.00 mL\nTube 3 → 1.00 mL] --> B5
        B5[Mix each solution with a stirring rod\nClean rod between tubes] --> B6
        B6[Transfer each solution into\nspectrophotometer test tube\nRinse 3x, fill 3/4, wipe outside] --> B7
        B7[Measure absorbance A\nfor all 3 solutions\nRecord values] --> B8
        B8[Discard solutions in waste containers\nRinse all glassware with DI water]
    end

    B8 --> POSTLAB

    subgraph POSTLAB ["📝 Post-Lab"]
        P1[Wipe bench, put away glassware] --> P2
        P2[Have TA sign and date data pages] --> P3
        P3[Complete post-lab report in Stemble\nDue: 11:59 pm on lab day]
    end

    POSTLAB --> END([✅ Experiment Complete])
