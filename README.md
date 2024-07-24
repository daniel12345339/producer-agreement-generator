<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Producer Agreement Generator</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #2c2c2c;
            color: #ffffff;
            padding: 20px;
        }
        .hidden {
            display: none;
        }
        label {
            display: block;
            margin-top: 10px;
        }
        input, select {
            width: 100%;
            padding: 10px;
            margin-top: 5px;
            margin-bottom: 20px;
            border: 1px solid #ccc;
            border-radius: 4px;
        }
        .section-title {
            font-size: 20px;
            margin-top: 20px;
        }
        .info {
            color: #aaa;
            font-size: 12px;
        }
    </style>
</head>
<body>
    <h1>Input Info To Generate Producer Agreement</h1>
    <p>This tool was designed by music executives to streamline production agreements for artists. As we know, not everyone has access to a top lawyer, so our goal is to democratize music legal for the next generation of artists.</p>
    <label for="artist-company">Does the artist have a company? <span class="info">If you have an artist company, corporation, or LLC, then select 'yes'. If not, select 'no'</span></label>
    <select id="artist-company" name="artist-company">
        <option value="no">No</option>
        <option value="yes">Yes</option>
    </select>
    
    <div id="artist-company-name-section" class="hidden">
        <label for="artist-company-name">What is the artist's company name? <span class="info">This is the name of Artist's company, LLC, or corporation</span></label>
        <input type="text" id="artist-company-name" name="artist-company-name">
    </div>

    <label for="producer-loanout">Does the producer have a loan-out company? <span class="info">If you have a producer company, corporation, or LLC, then select 'yes'. If not, select 'no'</span></label>
    <select id="producer-loanout" name="producer-loanout">
        <option value="no">No</option>
        <option value="yes">Yes</option>
    </select>

    <div id="producer-loanout-company-name-section" class="hidden">
        <label for="producer-loanout-company-name">What is the producer's loan-out company name?</label>
        <input type="text" id="producer-loanout-company-name" name="producer-loanout-company-name">
    </div>

    <label for="effective-date">What is the effective date? <span class="info">This means the day of the contract, which would likely be today or sometime this week</span></label>
    <input type="date" id="effective-date" name="effective-date">

    <label for="producer-legal-name">What is the producer's legal name? <span class="info">This is your government name</span></label>
    <input type="text" id="producer-legal-name" name="producer-legal-name">

    <label for="producer-professional-name">What is the producer's professional name? <span class="info">In other words, what does the world know you as, which can be different from your legal name</span></label>
    <input type="text" id="producer-professional-name" name="producer-professional-name">

    <label for="artist-legal-name">What is the artist's legal name?</label>
    <input type="text" id="artist-legal-name" name="artist-legal-name">

    <label for="artist-professional-name">What is the artist's professional name?</label>
    <input type="text" id="artist-professional-name" name="artist-professional-name">

    <label for="artist-address">What is the artist's address? <span class="info">Where should we send you payment / notice information</span></label>
    <input type="text" id="artist-address" name="artist-address">

    <label for="artist-contact-name">What is the artist's contact name? <span class="info">This can be your name or it can be your business manager, attorney, or a friend that helps you oversee business</span></label>
    <input type="text" id="artist-contact-name" name="artist-contact-name">

    <label for="artist-contact-email">What is the artist's contact email?</label>
    <input type="email" id="artist-contact-email" name="artist-contact-email">

    <label for="producer-address">What is the producer's address?</label>
    <input type="text" id="producer-address" name="producer-address">

    <label for="producer-contact-name">What is the producer's contact name? <span class="info">This can be your name or it can be your business manager, attorney, or a friend that helps you oversee business</span></label>
    <input type="text" id="producer-contact-name" name="producer-contact-name">

    <label for="producer-contact-email">What is the producer's contact email?</label>
    <input type="email" id="producer-contact-email" name="producer-contact-email">

    <label for="distributor-name">What is the name of the distributor for the song? <span class="info">This is where the song will be distributed. If you don't know, write "TBD"</span></label>
    <input type="text" id="distributor-name" name="distributor-name">

    <label for="composition-masters">Number of Masters</label>
    <input type="number" id="composition-masters" name="composition-masters">

    <label for="advance-amount">Advance Amount</label>
    <input type="number" id="advance-amount" name="advance-amount">

    <label for="advance-currency">Advance Currency</label>
    <select id="advance-currency" name="advance-currency">
        <option value="USD">USD</option>
        <option value="EUR">EUR</option>
        <option value="GBP">GBP</option>
        <!-- Add other currencies as needed -->
    </select>

    <label for="royalty-percent">Royalty Percent</label>
    <input type="number" step="0.01" id="royalty-percent" name="royalty-percent">

    <label for="governing-law">Governing Law</label>
    <select id="governing-law" name="governing-law">
        <option value="Alabama">Alabama</option>
        <option value="Alaska">Alaska</option>
        <option value="Arizona">Arizona</option>
        <option value="Arkansas">Arkansas</option>
        <option value="California">California</option>
        <option value="Colorado">Colorado</option>
        <option value="Connecticut">Connecticut</option>
        <option value="Delaware">Delaware</option>
        <option value="Florida">Florida</option>
        <option value="Georgia">Georgia</option>
        <option value="Hawaii">Hawaii</option>
        <option value="Idaho">Idaho</option>
        <option value="Illinois">Illinois</option>
        <option value="Indiana">Indiana</option>
        <option value="Iowa">Iowa</option>
        <option value="Kansas">Kansas</option>
        <option value="Kentucky">Kentucky</option>
        <option value="Louisiana">Louisiana</option>
        <option value="Maine">Maine</option>
        <option value="Maryland">Maryland</option>
        <option value="Massachusetts">Massachusetts</option>
        <option value="Michigan">Michigan</option>
        <option value="Minnesota">Minnesota</option>
        <option value="Mississippi">Mississippi</option>
        <option value="Missouri">Missouri</option>
        <option value="Montana">Montana</option>
        <option value="Nebraska">Nebraska</option>
        <option value="Nevada">Nevada</option>
        <option value="New Hampshire">New Hampshire</option>
        <option value="New Jersey">New Jersey</option>
        <option value="New Mexico">New Mexico</option>
        <option value="New York">New York</option>
        <option value="North Carolina">North Carolina</option>
        <option value="North Dakota">North Dakota</option>
        <option value="Ohio">Ohio</option>
        <option value="Oklahoma">Oklahoma</option>
        <option value="Oregon">Oregon</option>
        <option value="Pennsylvania">Pennsylvania</option>
        <option value="Rhode Island">Rhode Island</option>
        <option value="South Carolina">South Carolina</option>
        <option value="South Dakota">South Dakota</option>
        <option value="Tennessee">Tennessee</option>
        <option value="Texas">Texas</option>
        <option value="Utah">Utah</option>
        <option value="Vermont">Vermont</option>
        <option value="Virginia">Virginia</option>
        <option value="Washington">Washington</option>
        <option value="West Virginia">West Virginia</option>
        <option value="Wisconsin">Wisconsin</option>
        <option value="Wyoming">Wyoming</option>
    </select>

    <button onclick="generateAgreement()">Generate Agreement</button>

    <h2>Generated Agreement</h2>
    <div id="generated-agreement"></div>

    <script>
        document.getElementById('artist-company').addEventListener('change', function() {
            var value = this.value;
            document.getElementById('artist-company-name-section').style.display = value === 'yes' ? 'block' : 'none';
        });

        document.getElementById('producer-loanout').addEventListener('change', function() {
            var value = this.value;
            document.getElementById('producer-loanout-company-name-section').style.display = value === 'yes' ? 'block' : 'none';
        });

        function generateAgreement() {
            var artistCompany = document.getElementById('artist-company').value;
            var artistCompanyName = document.getElementById('artist-company-name').value;
            var producerLoanout = document.getElementById('producer-loanout').value;
            var producerLoanoutCompanyName = document.getElementById('producer-loanout-company-name').value;
            var effectiveDate = document.getElementById('effective-date').value;
            var producerLegalName = document.getElementById('producer-legal-name').value;
            var producerProfessionalName = document.getElementById('producer-professional-name').value;
            var artistLegalName = document.getElementById('artist-legal-name').value;
            var artistProfessionalName = document.getElementById('artist-professional-name').value;
            var artistAddress = document.getElementById('artist-address').value;
            var artistContactName = document.getElementById('artist-contact-name').value;
            var artistContactEmail = document.getElementById('artist-contact-email').value;
            var producerAddress = document.getElementById('producer-address').value;
            var producerContactName = document.getElementById('producer-contact-name').value;
            var producerContactEmail = document.getElementById('producer-contact-email').value;
            var distributorName = document.getElementById('distributor-name').value;
            var compositionMasters = document.getElementById('composition-masters').value;
            var advanceAmount = document.getElementById('advance-amount').value;
            var advanceCurrency = document.getElementById('advance-currency').value;
            var royaltyPercent = document.getElementById('royalty-percent').value;
            var governingLaw = document.getElementById('governing-law').value;

            var lenderText = producerLoanout === 'yes' ? producerLoanoutCompanyName : producerLegalName;

            var agreement = `
                <p>This agreement ("Agreement") dated as of ${effectiveDate} sets forth the material terms of the agreement between ${artistCompany === 'yes' ? artistCompanyName : artistLegalName} ("Company", "we" or "us") and ${lenderText} ("Lender" or "you") f/s/o ${producerProfessionalName} ("Producer") for Producer's non-exclusive services in connection with the master recording(s) set forth below featuring the recorded performance(s) of the artist professionally known as ${artistProfessionalName} ("Artist") recorded in connection with and/or for possible inclusion on, among other things, Artist's upcoming release (the "Release") subject to Company's distribution/recording agreement ("Distribution Agreement") with a ${distributorName} ("Distributor"). Capitalized terms used herein and not specifically defined herein shall have the meaning(s) ascribed to them in the Distribution Agreement; in the event of any discrepancy, the definitions set forth in this Agreement shall be deemed controlling. Lender and Company agree to the following:</p>
                <table border="1" cellpadding="5" cellspacing="0">
                    <tr>
                        <td>1. Artist</td>
                        <td>${artistLegalName} p/k/a ${artistProfessionalName}</td>
                    </tr>
                    <tr>
                        <td>2. Producer</td>
                        <td>${producerLegalName} p/k/a ${producerProfessionalName}</td>
                    </tr>
                    <tr>
                        <td>3. Artist Address</td>
                        <td>${artistAddress}<br>Contact Name: ${artistContactName}<br>Contact Email: ${artistContactEmail}</td>
                    </tr>
                    <tr>
                        <td>4. Producer Address</td>
                        <td>${producerAddress}<br>Contact Name: ${producerContactName}<br>Contact Email: ${producerContactEmail}</td>
                    </tr>
                    <tr>
                        <td>5. Composition(s) / Master(s)</td>
                        <td>${compositionMasters} master recordings ("Master(s)") embodying Artist's featured performance of the musical composition(s) listed on Schedule 1 (the "Composition(s)" and each a "Composition") attached hereto and made a part hereof.</td>
                    </tr>
                    <tr>
                        <td>6. Services</td>
                        <td>Producer shall perform all services in connection with the Master(s) as are customarily performed by producers in the recording industry. The Master(s) shall be commercially and technically satisfactory to both Company and Distributor for the manufacture and sale of records.</td>
                    </tr>
                    <tr>
                        <td>7. Advance</td>
                        <td>Company shall pay you an aggregate all-in advance of ${advanceAmount}${advanceCurrency} for ${compositionMasters} Master(s), which such Advance shall be deemed fully recoupable against Producer's Royalty (as defined below). The Advance will be paid in full promptly following the complete execution of this Agreement.</td>
                    </tr>
                    <tr>
                        <td>8. Royalty</td>
                        <td>Company shall pay or shall instruct and cause Distributor to pay or otherwise allocate (pursuant to the irrevocable letter of direction annexed hereto and incorporated by reference herein as Exhibit B) a royalty to Lender in the amount per Master of ${royaltyPercent}% of Net Artist Royalties (as defined in the "Producer Royalty Provisions", attached as Schedule 2 and made a part hereof) actually received by Company in connection with exploitations of the Masters hereunder on top-line USNRC net sales of records ("Producer's Royalty"). Producer's Royalty shall be calculated, determined, adjusted and reduced on the same basis (without regard to sales based escalations or Artist's overall recoupment status) as set forth in Exhibit A, and payment of Producer's Royalty shall be subject to the terms and conditions as embodied in the Producer Royalty Provisions and Exhibit A, as applicable. For the avoidance of doubt, in the event there is a discrepancy between the terms and conditions contained in Schedule 2 and the Distribution Agreement, the terms and conditions of the Distribution Agreement shall control. Producer's Royalty shall not be reduced by amounts payable to any third party producers or mixers who perform additional services with respect to the Master(s) unless such third parties were engaged by Producer, following satisfactory delivery and acceptance of the Master by Company and/or Distributor.</td>
                    </tr>
                    <tr>
                        <td>9. Controlled Composition</td>
                        <td>The parties acknowledge that the Composition(s) shall be owned and/or controlled in accordance with the ownership interests set forth on Schedule 1. In the event that any composition(s) which are wholly or partly written, owned or controlled by Lender, Producer, or Producer Personnel (hereafter defined) is embodied in the Master, Lender and Producer hereby irrevocably license (and shall use reasonable efforts to cause their and Producer Personnel's respective publishing designee(s) [each, a "Producer Publisher"] to license) their respective share(s), in and to the Composition(s) to Company, Artist, Distributor, and each of their respective designees, licensees, and assignees (sometimes referred to herein collectively as "Company's Designees") an irrevocable universe-wide first-use license under copyright to reproduce and exploit their respective share(s) in the Composition(s) as embodied on the Master at a rate equal to one hundred percent (100%) of the minimum statutory or prevailing rate in the United States and Canada, as applicable, as of the date of initial release of the Master(s) and without regard to so-called "caps" but otherwise pursuant, if applicable, to the so-called Controlled Composition clause contained in the Distribution Agreement Extracts. Further, Lender and/or Producer shall license and/or shall use reasonable efforts to cause their Producer Publisher(s) (and to cause Producer Personnel) to license to Company's Designees, a nonexclusive, worldwide and perpetual synchronization and other necessary use license(s), free of charge or royalty, solely for the purpose of reproducing Lender's and/or Producer's and/or Producer Personnel's share of any Composition in any promotional Video (as defined in the Distribution Agreement Extracts) and exhibiting, duplicating, manufacturing and distributing copies of such Video only in connection with promotional purposes and only in the event that Artist, any other co-writer's or publishing designees of the Composition do not receive any compensation for said promotional use. The foregoing is not intended to limit Lender's, Producer's, or any Producer Publisher's right to receive directly its respective share of publishing monies in connection with "monetized" promotional Videos (e.g., Videos exhibited on YouTube, Vimeo or Vevo). For the avoidance of doubt, each applicable writer/publisher shall exclusively administer his/her/its respective share of the applicable Composition(s) and to collect directly from the applicable sources only their respective share of income derived from the exploitation of the Composition(s).</td>
                    </tr>
                    <tr>
                        <td>10. Ownership of Master(s) / Grant of Rights</td>
                        <td>All results and proceeds of the services of Lender, Producer, and/or any third party furnished or engaged solely by Lender or Producer (hereinafter individually and collectively referred to as "Producer Personnel"), including the Master(s) (but excluding the Composition(s) to the extent of Lender's and/or Producer's interest therein and thereto) shall be deemed "works-for-hire" for Company within the meaning of the Copyright Act of 1976 (Title 17, U.S.C.), as amended, and subject to the provisions of this Agreement, and Lender shall cause any such Producer Personnel to be bound in writing by the terms hereof. If it is determined that the Master(s) do not so qualify, then the Master(s), together with all rights therein (other than the Composition(s)), shall be automatically assigned to Company and Company's Designees by this Agreement. For the avoidance of doubt, the parties hereto acknowledge that any co-producers of the Master has/have a producer agreement with Artist that is separate and apart from this Agreement with Producer, which delineates payments of any advances and royalties to such co-producer(s) and that such co-producer(s) shall not be considered "Producer Personnel" hereunder. Upon signature of this Agreement, Lender and Producer shall immediately transfer to Company all rights (including but not limited to copyright) in and to the Master(s) (excluding the Composition(s)). Lender and Producer further grant to Company and Company's Designees the right, throughout the universe and in perpetuity, to use Lender's name and Producer's professional name, and Producer's approved likeness and approved biographical material solely in the packaging and metadata of Records embodying the Master(s) and in all promotion and advertising therefor. We shall provide Lender for Lender's and/or Producer's approval any likeness, portrait or pictures of Producer or biographical material about Producer which we propose to use in connection therewith. We will not use any such material which Lender disapproves in writing within five (5) business days following the date on which such materials are received by Lender or Producer, provided Lender or Producer furnishes substitute material, satisfactory to us in our sole and reasonable discretion, in time for use within Distributor's production and release schedules. No inadvertent, non-repetitive failure to comply with this paragraph will constitute a breach of this Agreement provided that following written notice from Lender, Company cures and/or uses reasonable commercial efforts to cure or instruct Distributor or other applicable third parties to prospectively cure any such credit failure (and cure as promptly as possible with regard to DSP's) and Lender and Producer will not be entitled to injunctive relief to restrain the continuing use of any material used in contravention of this paragraph. Lender shall have the right to submit photographs and likenesses of, and biographical material concerning, Lender's submission of the same shall constitute Lender's and Producer's approval thereof. Lender shall cause Producer to waive any claims based on infringement of Producer's "moral rights", and understands that the Master(s) may be changed, altered, remixed, or coupled with any other recording(s) or other material in Company's and Distributor's sole discretion, subject to the terms and conditions of the Distribution Agreement. Lender and Producer shall have the right to request that Producer's credit be removed from the Master(s) if the Master(s) are materially altered in any way (other than for timing or formatting purposes) by giving Company written notice thereof. For avoidance of doubt, Producer is not an original author of the copyright underlying the Master(s) and shall not in any event claim any reversionary right under the United States Copyright Act Section 203, or otherwise.</td>
                    </tr>
                    <tr>
                        <td>11. Credit</td>
                        <td>With respect to the Master(s), Company shall accord, or shall instruct and use reasonable commercial efforts to cause Distributor to provide, credit to Producer as set forth on Schedule 1 on the labels, back cover, and in the liner notes of any record containing the Master(s) on metadata in connection with electronic transmissions, including any "single" embodying the Master(s) on the A-side, and in all print and consumer ads (including Billboard strip ads) placed or controlled by Company or Distributor of one-quarter (1/4) page or larger featuring the Master(s), provided, all other producers of the Master are credited the same. Company's inadvertent, non-repetitive failure, or any failure by Distributor, to provide such credit shall not be deemed to be a material breach of this Agreement, provided that following written notice from Lender, Company uses reasonable commercial efforts to cure or instruct Distributor or other applicable third parties to prospectively cure any such credit failure and as promptly as possible following the receipt of notice with regards to DSPs. In no event shall Lender or Producer be entitled to an injunction in connection with a breach of these credit provisions.</td>
                    </tr>
                    <tr>
                        <td>12. Samples</td>
                        <td>Lender and Producer will not "sample", "interpolate", or otherwise incorporate into ("Sample," "Sampling") the Master(s) or Composition(s) (if applicable), or permit any Producer Personnel to Sample any copyrighted or otherwise proprietary material ("Proprietary Material") belonging to any person, other than such material owned and/or supplied to Lender or Producer by Company or Artist for such purpose, unless approved by Company or Artist in writing. Lender shall advise us in writing of any such Proprietary Material solely incorporated by you and shall provide us with all information necessary to obtain appropriate permissions to use same, without restriction, on and in connection with the applicable Master(s). We shall have no obligation to accept any master recordings containing Proprietary Material, and our or Distributor's acceptance or use of same shall not relieve Lender and Producer of any obligations hereunder nor deprive us of any rights hereunder. Without limitation of Company's other rights: (a) in connection with any Approved Sample (as hereinafter defined), (i) any sums payable by or on behalf of Company or Company's Designees in connection with the clearance of Samples that have been disclosed to and approved by us in writing prior to commercial release of the applicable Master ("Approved Sample") shall be deemed additional recoupable recording costs, (ii) Lender and Producer shall be solely responsible for paying for an amount equal to any and all other recurring obligations and similar costs therefor (e.g., royalties or any contingency participation conveyed [whether expressed in royalty or penny-rate terms], etc.), multiplied by the Fraction (hereinafter defined), and (iii) any copyright ownership in the Composition that must be conveyed to a third party with respect to such Approved Sample shall be borne pro-rata by all writers; and (b) notwithstanding anything to the contrary contained herein, any sums payable (including, without limitation, record royalties) by or on behalf of Company or Company's Designees in connection with the clearance of Samples embodied by Lender, Producer, and/or Producer Personnel that have not been disclosed to and approved by us prior to commercial release of the applicable Master ("Undisclosed Sample") shall be deductible from any and all sums and/or interest due or accorded to Lender and/or Producer hereunder, and any copyright ownership in the Composition that must be conveyed to a third party with respect to such Undisclosed Sample shall be borne entirely by Lender, Producer, Producer Personnel and/or Producer Publisher, as applicable.</td>
                    </tr>
                    <tr>
                        <td>13. Indemnity / Governing Law / Venue</td>
                        <td>(a) Each party hereto agrees to indemnify and hold each other party's designees, licensees and assigns (collectively, the "Indemnified Party") from all damages, liabilities, out-of-pocket costs, losses and expenses (including legal costs and actual and reasonable outside attorney's fees) arising out of or connected with any third party claim, demand, or action which is inconsistent with any of the warranties, representations, or covenants made by such indemnifying party in this Agreement provided such claim is reduced to a final, adverse, non-appealable judgment or settled with the indemnifying party's prior written consent. The indemnifying party will reimburse the Indemnified Party upon written demand for any payment made by the Indemnified Party at any time in respect of any such third-party claim, liability, damage or expense to which the foregoing indemnity relates. The Indemnified Party shall give the indemnifying party prompt written notice of any claim to which the foregoing indemnity applies, and the indemnifying party may participate in the defense of same with counsel of its choosing at its sole cost and expense; provided that the Indemnified Party's decision in connection with the defense of any such claim shall be final.
                        (b) Company may withhold payments due to Lender pending resolution of any claim related to Lender's foregoing indemnity obligation, but if Lender posts a surety bond from a company approved by Company in its reasonable discretion (in an amount related to Lender's and/or Producer's potential liability), Company will not withhold such payments. Pending the determination of any claim relating to Lender's foregoing indemnity obligation, unless Lender posts a bond in a form and amount acceptable to Company in Company's reasonable discretion, Company shall have the right to withhold from any sums due Lender hereunder an amount equal to Lender's potential liability pursuant to this paragraph. If as of the date twelve (12) months following the date such sums were initially withheld, no litigation on the claim has commenced and no settlement discussion are then taking place, then the sums so withheld shall be credited to your account (subject to Company's right to once again withhold if litigation subsequently is instigated).
                        (c) If either party hereto institutes any action, suit or proceeding based upon any matter, claim or controversy arising hereunder or relating hereto, such action shall be brought solely in the State of ${governingLaw} and shall be governed by ${governingLaw} and the parties hereto (and Lender shall cause Producer to) submit to the jurisdiction and venue of said court, provided that notwithstanding anything to the contrary in this paragraph, if Company or Artist is sued or joined (e.g. by joinder or impleader) in any other court or forum by a person, or entity other than Lender or Producer in respect of any matter that may give rise to a claim by or against Lender or Producer hereunder, Lender consents (and shall cause Producer to consent) to the jurisdiction of such court or forum over any such claim asserted against Lender or Producer.
                        (d) Regardless of the form in which any action hereunder is pursued, and without limitation of the right of either party hereunder to pursue other lawful methods of service of process, service of process on the respective party in writing and which is either delivered (a) by Express Mail, Federal Express or other express delivery service (receipt requested), or (b) via registered or certified mail, return receipt requested and received, at the respective address set forth above, shall be deemed for all purposes personal service upon such party under the ${governingLaw} Rules of Civil Procedure and the Federal Rules of Civil Procedure, respectively.</td>
                    </tr>
                </table>
            `;

            document.getElementById('generated-agreement').innerHTML = agreement;
        }
    </script>
</body>
</html>
