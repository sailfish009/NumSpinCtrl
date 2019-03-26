
// copyright: Damir Valiulin : https://www.codeproject.com/articles/1310/cnumspinctrl-a-simple-numeric-spin-control
usage:

    CNumSpinCtrl m_spin[8];

    void CSampleDlg::DoDataExchange(CDataExchange* pDX)
    {
    	CDialogEx::DoDataExchange(pDX);
    	DDX_Control(pDX, IDC_SPIN1, m_spin[0]);
    	DDX_Control(pDX, IDC_SPIN2, m_spin[1]);
    	DDX_Control(pDX, IDC_SPIN3, m_spin[2]);
    	DDX_Control(pDX, IDC_SPIN4, m_spin[3]);
    	DDX_Control(pDX, IDC_SPIN5, m_spin[4]);
    	DDX_Control(pDX, IDC_SPIN6, m_spin[5]);
    	DDX_Control(pDX, IDC_SPIN7, m_spin[6]);
    	DDX_Control(pDX, IDC_SPIN8, m_spin[7]);
    }

    // ...
    m_spin[i].SetBuddy(GetDlgItem(nID));
 	  m_spin[i].SetDecimalPlaces(decimal);
	  m_spin[i].SetTrimTrailingZeros(FALSE);
	  m_spin[i].SetRangeAndDelta(min, max, delta);
	  m_spin[i].SetPos(pos);
